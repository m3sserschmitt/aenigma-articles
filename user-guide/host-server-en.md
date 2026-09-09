## Hosting a Server

Aenigma provides a simple way to host your own private messaging system right on
your personal device, for all desktop platforms: Windows, Mac, and Linux. This is
made possible through virtualization. Your device will become the host for a
virtual image of the system running Aenigma. Virtual images are currently
available for `Virtualbox` and `libvirt/Qemu`.

### Table of Contents

- [Installing the Virtual Machine](#installing-the-virtual-machine)
- [Tor Browser](#tor-browser)
- [Aenigma Mobile App](#aenigma-mobile-app)
- [Configuration](#configuration)
- [Setting a Password - Optional](#setting-a-password---optional)
- [Federation](#federation)
- [Other Features](#other-features)
- [Contact](#contact)

### Installing the Virtual Machine

Go to [aenigma-boxes](https://github.com/m3sserschmitt/aenigma-boxes)
and follow the steps required to install the virtual image described in the
[README.md](https://github.com/m3sserschmitt/aenigma-boxes/blob/gh-pages/README.md)
document. From here on, we will assume the user has successfully installed the
virtual image and successfully established a connection to the Aenigma virtual
machine.

### Tor Browser

Aenigma works over [TOR](https://en.wikipedia.org/wiki/Tor_(network)), a network
maintained by volunteers around the world that enables anonymization. In
addition, it allows us to host services without registering our own internet
domain and without exposing personal equipment on the internet. As a
consequence, services hosted through TOR can only be accessed using specialized
software. One such piece of software is
[Tor Browser](https://www.torproject.org/download/), which must be installed
to successfully complete the configuration.

### Aenigma Mobile App

The [Aenigma mobile app](https://play.google.com/store/apps/details?id=ro.aenigma)
integrates [tor-android](https://github.com/guardianproject/tor-android), a
native Android library that enables communication over the TOR network. Visit
this
[document](https://github.com/m3sserschmitt/aenigma-articles/blob/gh-pages/user-guide/contacts-screen-ro.md)
to understand how Aenigma can establish a connection over the TOR network to
the private server that is about to be configured.

### Configuration

In the directory where
[aenigma-boxes](https://github.com/m3sserschmitt/aenigma-boxes) was cloned
(from the [Installing the Virtual Machine](#installing-the-virtual-machine)
step), open a command line and connect to the Aenigma virtual machine using the
following command:

```bash
vagrant ssh
```

After successfully connecting, the following message will be visible on the
command line:

![alt text](./images/server-status.png)

Initially, the virtual machine will have two services configured:
`aenigma-dashboard` (for administration) and `aenigma` (used by the
[Aenigma mobile app](#aenigma-mobile-app) to connect to the server). While the
`aenigma` service is accessible to anyone who has the address, `aenigma-dashboard`
is protected by an access key. Copy the address of the `aenigma-dashboard`
service and open Tor Browser. In the address bar, enter the copied address
adding `/dashboard`, as shown in the following image:

![alt text](./images/server-dashboard-auth.png)

To obtain the access key you can use the command

```bash
sudo sudo aenigma-tor-get-auth -s aenigma-dashboard -u aenigma-dashboard
```

as in the following example:

![alt text](./images/server-get-auth.png)

Only the characters after `x25519` should be entered into Tor Browser for
authentication. After obtaining the access key, you can access the server's
administration page through Tor Browser.

> __*Note*__: You can check *`Remember this key`* to make future connections
> faster.

> __*Note*__: Create a bookmark for this page to make future access easier.

![alt text](./images/server-dashboard.png)

On this page we can observe the following:

1. The server password input field. It is not configured initially and the
field is inactive. The service can function without a password being
configured, but it is recommended that the administrator go through this step.
See [setting a password](#setting-a-password---optional).
2. The connection QR code. It can be scanned directly from the Aenigma mobile
app for a direct connection. It can be shared with other people for
connecting. Visit this
[document](https://github.com/m3sserschmitt/aenigma-articles/blob/gh-pages/user-guide/servers-bottom-sheet-ro.md)
to learn how a connection to the server can be established from the
[Aenigma mobile app](#aenigma-mobile-app).
3. The connection details for federation purposes. They can be shared with
other people who administer Aenigma servers in order to form a federation. In
this scenario, multiple servers communicate with one another and users can
exchange messages even when they are not connected to the same server. See
[Federation](#federation) for more information.
4. The area for entering another server's connection details, for federation
purposes.
5. The list of servers with which an active connection exists.

> __*Important*__: The connection between servers must __not__ be made in both
> directions. If you share the connection details (from section 3 of the
> `/dashboard` page) with another person for the purpose of connecting, then
> you __do not__ need to connect in the opposite direction as well. One party
> shares, the other initiates the connection.

### Setting a Password - *Optional*

Initially the server operates without a password - the Aenigma service will
start automatically when the virtual machine starts. It is highly recommended
that a password be configured to protect the server's private keys. This can
be done very easily using the command

```bash
sudo aenigma-lock-key
```

> __*Note*__: As the password characters are typed, they will not be displayed
> on screen. This is a standard privacy protection measure.

after which the service is restarted using the command

```bash
sudo aenigma-start
```

as in the following example:

![alt text](./images/server-lock-key.png)

> After configuring a password, the `/dashboard` page must be checked through
> Tor Browser at every startup. If the password field is *active* and allows
> characters to be entered, then the password *must* be entered. An *inactive*
> field indicates that the password does *not* need to be entered.

### Federation

For small groups of users, setting up a single private server is easy and does
not require significant resources. For larger groups or multiple groups
acting independently, a single server shared by all users is not sufficient.
In this case, each group can set up its own communication server and then
configure connections between them. The *federation* is therefore the
totality of servers between which there is a direct or even indirect link for
the purpose of exchanging information.

> __*Example:*__ Three independent groups each set up their own private
> communication server: *A*, *B*, and *C*. We could have the links *A-B*,
> *A-C*, and *B-C* - each node is connected to the other two. However, the
> variant with only the links *A-B* and *B-C* is also valid and fully
> functional, because nodes *A* and *C* will communicate through *B*. This can
> be similarly extended to 4, then 5, and so on.

By establishing these connections, messages are synchronized between the
participating nodes, and users can communicate even when they are not
connected to the same node.

### Other Features

The [Aenigma suite](https://github.com/m3sserschmitt/aenigma-packages) contains
a multitude of other features, including:

```bash
aenigma-config
aenigma-tor-auth
aenigma-keys
aenigma-tor-get-auth
aenigma-launcher
aenigma-unlock-key
aenigma-lock-key
aenigma-update
aenigma-proxy
aenigma-vpn-client
aenigma-standard-setup
aenigma-vpn-dns
aenigma-start
aenigma-vpn-server
aenigma-status
aenigma-vpn-server-client
aenigma-tor
aenigma-vpn-server-host
```

For each of these, you can access the help page through

```bash
man aenigma-config
man aenigma-tor-auth
...
```

### Contact

You can report bugs or suggest improvements at [contact@aenigma.ro](mailto:contact@aenigma.ro)