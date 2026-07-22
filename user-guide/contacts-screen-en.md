## The Contacts List Screen

On this screen the user can access their contact list. Here they can also
resynchronize with the server, connect to a different server, and share the
current location with the entire contact list. The system does not implement any
automatic mechanism for synchronizing the current location. When the user connects to
another server, their contacts will not be automatically informed. This decision is
intentional and is meant to protect the user. Only they decide when to make
the server they are connected to known, in order to receive messages from other
users. The application allows connecting through the public internet, to
public domains, e.g., *aenigma.ro*, as well as connecting to location hidden services,
e.g., *.onion* sites. For the latter, it is necessary to use the
TOR or Orbot service, as described below.

![alt text](https://articles.aenigma.ro/user-guide/images/contacts-screen.png)

1. The button for showing/hiding the list of available servers.
2. The resynchronization button with the server. The connection will be rebuilt from the start.
This can be used in situations where message delivery is delayed or completely failed.
3. The search button for the contact list.
4. The access button for information.
5. The button for showing/hiding the secondary menu.
6. The button for enabling/disabling the Onion Routing service. The application allows
connecting through the TOR network, so the connection passes through multiple IP
addresses (servers maintained by volunteers around the world) until it reaches the selected server.
This is useful for protecting the user's current location and for anonymization. It also allows
connecting to location hidden services, i.e., *.onion* sites. Visit
[https://www.torproject.org/](https://www.torproject.org/) for additional
information.
7. Similarly, the application can also make connections through Orbot. This is
a VPN-type application that allows connecting to the TOR network. It requires installation from Google Play, but the necessary configuration is extremely simple and fast.
8. The button for enabling/disabling the notification service. The application implements
an independent synchronization and notification system for when it is not being used
or the device screen is off (i.e., the application is in the *background*).
9. Navigation to the screen with details about the application.
10. The navigation button for adding a new contact.
11. The handle used to access/dismiss, by swiping, the list of available servers.

### Server List

By pressing the button to show the server list, or by swiping using the
handle at the bottom of the screen, the list of available servers can be made
visible, as follows:

![alt text](https://articles.aenigma.ro/user-guide/images/contacts-screen-servers-bottom-sheet.png)

1. The resynchronization button with the server. The connection will be rebuilt from the start.
This can be used in situations where message delivery is delayed or completely failed.
2. The button for broadcasting the current location. When the user chooses a different server from
the list, their contacts will not be automatically notified. By pressing this
button, a message is sent to all contacts in the list. This way,
the user will still be able to receive messages from their contacts. Also,
messages received while the user is connected to a different location will be
automatically synchronized when they return to the original location (in case
they decide not to make their new location known).
3. The button for scanning the server's QR code. Users who choose to
manage their own server will be able to scan the QR code from the *"Dashboard"* page for
quick connection.
4. The access button for information.
5. The button for sharing the server address.
6. The server search field. Besides its search role, the field allows
connecting to addresses that are not listed. The user can enter any address,
and the connection will start when the "Connect" button is pressed.
7. The search button for the server list. Pressing it will start the search,
and the results will be displayed in the list.
8. The connect button. The application will attempt to connect to the entered address.
9. Allows the user to navigate to the list of available servers.
10. Allows the user to navigate to the list of servers they have connected to in the past.
11. The handle used to access/dismiss, by swiping, the list of available servers.

**Note**: *When the search button (i.e., the magnifying glass button) is used, the application
will search among the listed servers. When the "Connect" button
is used, it will attempt to connect to the entered address.*

### Selection Mode

By long-pressing on any contact in the list, a series of actions will become
available, as follows:

![alt text](https://articles.aenigma.ro/user-guide/images/contacts-screen-selection-mode.png)

1. The button for exiting selection mode.
2. The search button for the contact list.
3. The button for deleting the selected contact.
4. The button for editing the selected contact (e.g., renaming it).
5. The button for sharing the selected contact, with other contacts or via link.
6. The button for creating a chat group. There is no strict limit on the number of
participants in a group, but technical limitations will make message delivery
slower as their number grows considerably (hundreds or even thousands of
participants).
7. The contact selection indicator. In selection mode, simply tapping a
contact will cause it to be selected or, as appropriate, deselected.
8. The handle used to access/dismiss, by swiping, the list of available servers.
9. The navigation button for adding a new contact.

### Contact

You can report errors or suggest improvements at [contact@aenigma.ro](mailto:contact@aenigma.ro)