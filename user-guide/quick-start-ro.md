## Generalități

Acest document reprezintă un accesibil punct de start în utilizarea Aenigma. Sunt
descrise scurt și concis care sunt problemele pe care acest proiect își propune să le
rezolve. În final până și utilizatorul nefamiliarizat cu tehnologia va avea o imagine
de ansamblu asupra modului în care să își configureze propriul sistem de comunicare
criptat pe dispozitivele personale.

### Ceva ce știm? Sau poate am auzit din povești?

Înainte de mijloacelor electronice de comunicare, se foloseau scrisori.
O foaie de hârtie pe care este scris un mesaj ce mai apoi este împachetat într-un plic.
Pentru ca mesajul să ajungă la destinatar, plicul va trebui să aibă scris pe el adresa.
Nu uităm că, pentru a primi un răspuns, trebuie să scriem și adresa proprie pe spatele
plicului. Lipim plicul cu atenție iar mai apoi este înmânat serviciului poștal din
proximitatea noastră. Din aproape în aproape, trecând prin multiple oficii și centre de 
sortare, mesajul nostru ajunge la destinatar.

### Echivalentul digital

Aenigma funcționeză precum poșta (sau serviciul de curierat). Preia un *"plic"* pe care
îl livrează la o *"adresă"*. Ce poate totuși să facă în plus față de servicul național
de poștă este să mute poșta în computerul personal. Echivalentul mesajului scris pe
hârtie devine un șir de biți. Plicul este înlocuit de criptare. Adresele devin adrese de
internet. Oficiul poștal și centrele de sortare sunt înlocuite de servere.

### Anonimizarea? Înapoi la poștă.

Să presupunem că doi amici vor să cumunice și în același timp identitatea lor să rămână
necunoscută. În exemplul inițial cu poșta este imposibil. Adresele celor doi sunt la
vedere. Exită totuși un mic truc ce poate fi folosit pentru a induce în eroare
instituția poștală. Să presupunem că acești doi pasionați mai au alți trei
prieteni dispuși să ajute. În total vor fi cinci. Mesajul trebui să ajungă de la amicul
1 la amicul 5.

Amicul 1 scrie mesajul, îl introduce în plic și scrie pe acesta adresa
amicului 5. Apoi introduce plicul într-un al doilea plic pe care scrie adresa amicului
4, pe care îl introduce în alt plic pe care scrie adresa amicului 3, pe care îl
introduce în alt plic pe care scrie adresa amicului 2. Acest ultim plic ajunge prin
poștă la amicul 2 și este desfăcut. În interior se află plicul pe care se află adresa
amicului 3. Amicul 3 primește plicul, îl desface iar în interior se află plicul pe care
se află adresa amicului 4. Acesta din urmă, după primirea plicului, va desface și va
găsi plicul inițial pe care se află adresa amicului 5, destinația finală.

Excepția care iese imediat în evidență este faptul
ce amicii nu își mai scriu propria adresă pe plicuri. Mesajul nu se mai poate intoarce
dacă una dintre adrese nu poate fi găsită. Totuși, amicul 1, cel care a scris mesajul
inițial, va avea grijă sa menționeze în scrisoarea către amicul 5:


> *"...te rog să îmi răspunzi la adresa X.*
>
> *Cu drag,*
>
> *Amicul 1."*

Amicul 5 va proceda la fel, în sens invers, pentru a comunica cu amicul 1.

Aenigma este echivalentul digital al acestui truc. Fiecare amic are la dispoziție un 
computer personal conectat cu ceilalți amici. Mesajul este protejat prin straturi
succesive de criptare ce sunt îndepărtate unul câte unul, pe măsură ce mesajul merge,
din aproape în aproape, către destinatarul final. Este de observat că în acest
aranjament nu știe nimeni cine este persoana care a scris, respectiv cea care a citit
mesajul - cu excepția amicilor care s-au vorbit să pună la cale acest truc.

### Scopul?

Scopul imediat al acestui proiect este acela de a oferi o alternativă independentă de
comunicare privată. Cu siguranță există și alte alternative, cel puțin la
fel de ambițioase și de încredere. Totuși, ceea ce Aenigma își propune să realizeze este
o democratizare a comunicațiilor - de a pune în mâna celor cu resurse limitate
posibilitatea de a comunica neîngradit, necenzurat, liber de imperativa comercială.

### Cum se face?

Aenigma este disponibilă în
[Google Play](https://play.google.com/store/apps/details?id=ro.aenigma).
Pentru dispozitive lipsite de Servicii Google se poate folosi acest
[link](https://github.com/m3sserschmitt/aenigma-android/releases/latest/download/aenigma.apk).
Aplicația va avea un server public (sau mai multe, în funcție de posibilități) la care
se conectează inițial. *"Public"* nu nu presupune compromis în materie de securitate.
Inseamnă ca este disponibil la liber pentru toată lumea. Există și posibilitatea
găzduirii propriului server Aenigma folosind propriul echipament de acasă - un simplu
computer personal și o conexiune pe cât posibil stabilă la internet vor fi suficiente.
Diferite grupuri de acțiune vor găsi poate mai convenabilă varianta din urmă.

<a href="https://play.google.com/store/apps/details?id=ro.aenigma">
<img alt="Get it on Google Play"
src="https://play.google.com/intl/en_us/badges/static/images/badges/en_badge_web_generic.png"
width="150">
</a>

În continuare urmăriți seria de ghiduri rapide pentru a vă familiariza:

1. [Ghid de utilizare al aplicatiei mobile Aenigma](https://web.aenigma.ro/#/blog/article?url=https%3A%2F%2Farticles.aenigma.ro%2Fuser-guide%2Fquick-start-mobile-app-ro.md)
2. [Găzduiți propriul server Aenigma](https://web.aenigma.ro/#/blog/article?url=https%3A%2F%2Farticles.aenigma.ro%2Fuser-guide%2Fhost-server-ro.md)

### Contact

Puteți semnala erori sau propune îmbunătățiri la
[contact@aenigma.ro](mailto:contact@aenigma.ro)

---

*Acest document este licențiat sub
[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).*
