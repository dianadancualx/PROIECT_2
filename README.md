# PROIECT_2
Proiect Cloud 2 API realizat in Python cu Flask Framework

1. Descriere aplicație	
2. Descriere servicii API utilizate	
3. Implementare sistem	
4. Prezentare aplicație	


1. Descriere aplicație
Termenul de API este acronimul de la ApplicationPrograming Interface, care în limba română se poate traduce ca interfață de programare a aplicațiilor si reprezintă un set de reguli si specificații cu ajutorul cărora un program poate accesa si folosi resursele oferite de un alt program. Cu alte cuvinte, un program care oferă API-uri permite altor programe sa interacționeze cu acesta automat, de la program la program sau de la program la sistem de operare, fără sa fie nevoie de folosirea unei interfețe grafice de utilizare (GUI) si fără cunoștințe legate de arhitectura sau elemente de programare ale programului ci doar folosirea specificațiilor de utilizare a API-ului oferit.

Lucrul cu API-uri este foarte folosit si in mediul online, o mulțime de aplicații web furnizează accesul la serviciile oferite prin intermediul unor seturi de reguli de comunicare bine precizate. Exemple de API-uri folosite in mediul online:
•	Google Maps API - permite dezvoltatorilor web sa incorporeze hărți in paginile web folosid cod JavaScript sau Flash;
•	YouTube API - permite incorporarea de videoclipuri de pe YouTube pe site-uri externe acestuia;
•	Flickr API - folosirea pozelor distribuite de o comunitate Flickr;
Putem sa ne referim la un API Web ca la un set de functii instalat pe un server separat si care poate fi apelat de un client pentru a prelua date. Un plus este faptul ca serverul poate stoca seturi immense de date care nu trebuie descarcate pentru a fi utilizate, cid oar sa apelam prin intermediull unui request doar obiectul care ne intereseaza. 

Aplicatia web creata in Python realizeaza interactiunea cu 2 API-uri pe baza unor requesturi si chei de conectare pentru a accesa datele oferite de aceste interfete fara a fi nevoie de a fi salvate initial local. Aplicatia afiseaza date despre starea curenta a vremii si localizarea pe harta pentru anumite puncte geografice oferite ca input.

2. Descriere servicii API utilizate
Pentru realizarea aplicației s-au utilizat 2 API-uri:
	Open Weather Map API: https://openweathermap.org/api 
Acest API este gratuit si simplu de utilizat, contine date despre starea vremii curente, forecast pentru vreme si date istorice ale vemii pentru un anumit oras/ pozitionare georgrafica. Accesul la datele oferite se utorizeaza pe baza unei chei in urma logarii in interiorul site-ului. 
	Google Maps API: https://developers.google.com/places/web-service/intro 
Cu ajutorul Google Maps API putem incorpora in aplicatiile noastre hartile online oferite de Google Maps. Pentru a avea acces la detaliile oferite despre anumite locatii (deschidere harta online, returnare latitudine/longitudine, adresa) putem apela acest API prin intermediul unui java script. 

3.Implementarea sistemului
Aplicatia de interactiune cu cele 2 API-uri este o aplicatie web si a fost implementata in cadrul pachetului software Microsoft Visual Studio Code folosind limbajul de programare Python. Stocarea datelor nu a fost necesara intrucat accesul la date a fost asigurat prin requesturile transmise de aplicatie catre API-uri. Alte tehnologii folosite pentru crearea aplicatiei au fost: HTML si Javascript. 
Python este un limbaj de programare dinamic multi-paradigmă, creat în 1989 de programatorul olandez Guido van Rossum. Python este un limbaj multifuncțional folosit de exemplu de către companii ca Google sau Yahoo! pentru programarea aplicațiilor web, însă există și o serie de aplicații științifice sau de divertisment programate parțial sau în întregime în Python. Se pune accentul pe curățenia și simplitatea codului, iar sintaxa sa le permite dezvoltatorilor să exprime unele idei programatice într-o manieră mai clară și mai concisă decât în alte limbaje de programare ca C. În ceea ce privește paradigma de programare, Python poate servi ca limbaj pentru software de tipul object-oriented, dar permite și programarea imperativă, funcțională sau procedurală. 

4. Prezentare Aplicație.
Structura proiectului:
Figura 1 – Structura proiectului
Pentru partea de frontend am folosit urmatoarele fisiere HTML: index.html, temperatures.html, layout.html.
Figura 2 – index.html
Figura 3 – temperature.html
Figura 4 – layout.html
Aplicatia Python este app.py, iar key.py contine cheia catre Google Maps API. Fisierul javascript script.js trimite requestul catre Google Maps API si incarca dupa ce requestul a fost realizat cu success tot continutul intr-un link.
Figura 5 –app.py
Figura 6 – app.py
Figura 7 – key.py
Figura 8 – script.js

Prezentarea aplicației
La rularea aplicatiei se deschide pagina HTML unde putem introduce ca parametru orasul pentru care vrem sa aflam informatiile curente despre starea vremii. Se trimite un request catre API-ul Open Weather Map si in functie de numele furnizat in textbox, dupa apasarea butonului “Submit” ni se vor returna datele corespunzatoare intr-un tab nou.
Figura 9 – Furnizare oras. Starea vremii
Figura 10 – Detalii. Starea Vremii
La accesarea noii ferestre se va deschide pagina pentru a căuta o locație cu ajutorul lui Google Maps API. Se cere ca parametru numele locației care va fi conectat cu un “place_id”  (parametru existent in fișierul json al API-ului) in urma apăsării butonului “Search”. Pentru a deschide harta locatiei Google Maps trebuie sa apăsam butonul “Click for Result!” si se va încărca harta online cu toate detaliile corespunzătoare
Figura 11 – Furnizare locație. Localizare
Figura 12 – Harta online. Localizare

 


