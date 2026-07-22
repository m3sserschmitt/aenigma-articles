## Ecranul listei de contacte

În acest ecran utilizatorul poate accesa lista sa de contacte. Tot aici se poate
efectua resincronizarea cu server-ul, conectarea la un server diferit și distribuirea
locației curente către întreaga listă de contacte. Sistemul nu implementează niciun
mecanism automat de sincronizare a locației curente. Când utilizatorul se conectează la un
alt server, contactele sale nu vor fi informate în mod automat. Această decizie este
intenționată și are ca scop protejarea utilizatorului. Doar acesta decide când își face
cunoscut server-ul la care este conectat pentru a putea primi mesaje de la alți
utilizatori. Aplicația permite conectarea prin intermediul internetului public, la
domenii publice, e.g., *aenigma.ro*, cât și conectarea la servicii cu locație ascunsă,
e.g., site-uri *.onion*. Pentru cele din urmă este necesară utilizarea serviciului
TOR sau Orbot, așa cum este prezentat în continuare.

![alt text](https://articles.aenigma.ro/user-guide/images/contacts-screen.png)

1. Butonul de afișare/ascundere a listei de servere disponibile.
2. Butonul de resincronizare cu server-ul. Conexiunea va fi refăcută de la început.
Se poate folosi în situații în care livrarea mesajelor este întârziată sau complet eșuată.
3. Butonul de căutare în lista de contacte.
4. Butonul de access pentru informații.
5. Butonul de afișare/ascundere a meniului secundar.
6. Butonul de activare/dezactivare a serviciului Onion Routing. Aplicația permite
conectarea prin rețeaua TOR, astfel conexiunea trece prin multiple adrese IP
(servere intrețiunute de voluntari în întreaga lume) până ajunge la server-ul selectat.
Este util pentru protejarea locației curente a utilizatorului și anonimizare. Permite, de
asemenea, conectarea de servicii cu locatie ascunsă, i.e., site-uri *.onion*. Accesați
[https://www.torproject.org/](https://www.torproject.org/) pentru informații
suplimentare.
7. Similar, aplicația poate realiza conexiuni și prin intermediu Orbot. Aceasta este
o aplicație tip VPN ce permite conectarea la rețeaua TOR. Necesită instalare din Google Play dar configurarea necesară este extrem de simplă și rapidă.
8. Butonul de activare/dezactivare a serviciului de notificări. Aplicația implementează
un sistem independent de sincronizare și notificare atunci când aceasta nu este folosită
sau ecranul dispozitivului este închis (i.e. aplicația se află în *background*).
9. Navigare către ecranul cu detalii despre aplicație.
10. Butonul de navigare către adăugarea unui nou contact.
11. Mânerul prin care se poate accesa/înlătura, prin glisare, lista de servere
disponibile.

### Lista de servere

Prin apăsarea butonului de afișare a listei de servere sau prin glisare cu ajutorul
mânerului din partea de jos a ecranului, se poate face vizibilă lista cu servere
disponibile, după cum urmează:

![alt text](https://articles.aenigma.ro/user-guide/images/contacts-screen-servers-bottom-sheet.png)

1. Butonul de resincronizare cu server-ul. Conexiunea va fi refăcută de la început.
Se poate folosi în situații în care livrarea mesajelor este întârziată sau complet eșuată.
2. Butonul de broadcast a locației curente. Când utilizatorul alege alt server din
listă, contactele acestuia nu vor fi notificate în mod automat. Prin apăsarea acestui
buton, un mesaj este transmis către toate contactele din listă. În acest fel
utilizatorul va putea primi în continuare mesaje de la contactele sale. De asemenea,
mesajele primite cât timp utilizatorul este conectat la o altă locație vor fi
sincronizate automat atunci cand acesta revine la locația inițială (în cazul în care
decide să nu își facă cunoscută noua locație).
3. Butonul de scanare a codului QR al server-ului. Utilizatorii care aleg să își
administreze propriul server vor putea scana codul QR din pagina *"Dashboard"* pentru
conectare rapidă.
4. Butonul de access pentru informații.
5. Butonul de distribuire a adresei server-ului.
6. Câmpul de căutare a server-ului. Pe langă rolul de căutare, câmpul permite
conectarea la adrese care nu sunt listate. Utilizatorul poate introduce orice adresă
iar conexiunea va începe la apăsarea butonului "Conectare" / "Connect".
7. Butonul de căutare în lista de servere. La apăsarea acestuia se va începe căutarea
și rezultatele vor fi afișate în listă. 
8. Butonul de conectare. Aplicația va încerca conexiunea la adresa introdusă.
9. Permite utilizatorului navigarea către lista de servere disponibile.
10. Permite utilizatorului navigarea către lista de servere la care a fost conectat în trecut.
11. Mânerul prin care se poate accesa/înlătura, prin glisare, lista de servere
disponibile.

**Notă**: *Atunci când se folosește butonul de căutare (i.e., butonul lupă), aplicația
va căuta în server-ele listate. Când se folosește butonul "Conectare" / "Connect"
se va încerca conectarea la adresa introdusă.*

### Modul selecție

Prin apăsarea lung o oricărui contact din listă, o serie de acțiuni vor deveni
disponibile, după cum urmează:

![alt text](https://articles.aenigma.ro/user-guide/images/contacts-screen-selection-mode.png)

1. Butonul de ieșire din modul selecție.
2. Butonul de căutare în lista de contacte.
3. Butonul de ștergere a contactului selectat.
4. Butonul de editare a contactului selectat (e.g., redenumirea acestuia).
5. Butonul de distribuire a contactului selectat, către alte contacte sau prin link.
6. Butonul de creare a unui grup de chat. Nu există o limită fermă pentru numărul de
participanți într-un grup, însă limitările tehnice vor face livrarea mesajelor mai
lentă pe măsură ce numărul acestora crește considerabil (sute sau chiar mii de
participanți).
7. Indicatorul de selecție a contactului. În modul selecție, simpla apăsare pe un
contact va cauza ca acesta să fie selectat sau, după caz, deselectat.
8. Mânerul prin care se poate accesa/înlătura, prin glisare, lista de servere
disponibile.
9. Butonul de navigare către adăugarea unui nou contact.

### Contact

Puteți semnala erori sau propune îmbunătățiri la [contact@aenigma.ro](mailto:contact@aenigma.ro)