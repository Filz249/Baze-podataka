## PRVI KOLOKVIJ

<details>
<summary><strong>1. Što je baza podataka?</strong></summary>
  
**Baza podataka** je skup istovrsnih podataka s višestrukom namjenom. Korisnik nije zainteresiran za sve vrste podataka u bazi, već samo za one koji su mu potrebni u njegovom poslu. Korisnik može imati uvid u samo jednu, njemu potrebnu datoteku koja ima uvijek istu i to vrlo jednostavnu strukturu, iako je u biti izvedena iz mnogo kompleksnije strukture podataka. Različiti korisnici uzimaju u obzir različite datoteke izvedene iz iste baze podataka.
</details>


---
<br>
<br>

<details>
<summary><strong>2. Zajedničke osobine za sve sustave baza podataka.</strong></summary>
  
- Apstraktni model podataka 
- Visoka razina pristupa ili upitnih jezika 
- Upravljanje transakcijama u višekorisničkom okruženju 
- Kontrola pristupa i vlasništvo nad podacima 
- Validacija podataka i provjera konzistentnosti 
- Konzistentni oporavak podataka nakon ispada sustava i/ili strojne opreme

</details>

---
<br>
<br>

<details>
<summary><strong>3. Nabrojite faze razvoja baze podataka.</strong></summary>
  
- Zahtjevi (analiza)
- Dizajn
- Implementiranje

</details>

---
<br>
<br>

<details>
<summary><strong>4. Nabrojite tri razine baze podataka.</strong></summary>

**1. Konceptualna razina**  
- predstavlja logički pogled na čitavu bazu podataka, preslikani model organizacije.

**2. Korisnička (vanjska) razina**  
- individualni korisnički pogled na bazu podataka, razvija se sukladno potrebama korisnika, može se razlikovati od sheme baze podataka.

**3. Fizička (unutarnja) razina**  
- implementiranje baze podataka na konkretnom hardveru, fizička pohrana podataka na mediju.

</details>

---
<br>
<br>

<details>
<summary><strong>5. Nabrojite osnovne tipove funkcija SUBP-a.</strong></summary>
  
- Aplikacija (engl. software) je sposobna upravljati radom jedne ili više baza podataka
- Mora osigurati stvaranje i održavanje sve tri razine baze podataka, kao i njihovo međusobno preslikavanje
- Reorganiziranje unutarnje ili fizičke razine bez mijenjanja logičke tj. konceptualne sheme
- Promjenu konceptualne sheme bez mijenjanja postojeće vanjske sheme.
  
</details>

---
<br>
<br>

<details>
<summary><strong>6. Nabrojite modele baza podataka.</strong></summary>

1. Hijerarhijske
2. Mrežne
3. Relacijske
4. Relacijske baze s objektno orijentiranim proširenjima
5. Objektno orijentirane baze podataka

</details>

---
<br>
<br>

<details>
<summary><strong>7. Navedite osnovne postupke apstrakcije.</strong></summary>
  
**1. Klasifikacija**
- Klasificiranje, opis i grupiranje entiteta u klase, razrede, odnosno tipove prema zajedničkim obilježjima. Opisuje se vezom (odnosom) “jest pojava” (engl. instance of).
 
**2. Generalizacija**
- Tipovi entiteta niže razine uopćuju se tipom entiteta više razine (nadtip i podtip). Opisuje se vezom “jest” (engl. is a).

**3. Agregacija**
- Formiranje novog pojma, višeg stupnja, na temelju odnosa postojećih pojmova.
  
</details>

---
<br>
<br>

<details>
<summary><strong>8. Što su to entitet, veza i atribut?</strong></summary>
  
**1. Entitet** je stvar, objekt, od značaja, realan ili imaginaran za koji je potrebno poznavati i čuvati određene informacije.

**2. Atribut** je svaki detalj koji služi da pobliže odredi, identificira, klasificira, kvantificira ili izrazi stanje entiteta.

**3. Veza** je agregacija/povezivanje dvaju ili više entiteta u novi entitet – vezu koji može imati i svoje atribute.

</details>

---
<br>
<br>

<details>
<summary><strong>9. Što čini relaciju?</strong></summary>
  
1. Zaglavlje od r je zaglavlje n-torke.

- Relacija r ima iste atribute i isti stupanj kao i zaglavlje.

3. Tijelo od r je skup n-torki koje sve imaju isto zaglavlje, kardinalnost n-torki je i kardinalnost od r.
  
</details>

---
<br>
<br>

<details>
<summary><strong>10. Što su to ključevi relacije i navedite ih?</strong></summary>
  
**Ključevi relacije** u relacijskoj bazi podataka su atributi ili skup atributa koji služe za jedinstveno identificiranje svake n-torke u relaciji.

**1. Super ključ** - atribut ili skup atributa koji jedinstveno određuje n torku unutar relacije.

**2. Kandidat ključ** - super ključ takav da nema nijedan odgovarajući podskup koji bi bio super ključ unutar relacije.

**3. Primarni ključ** - kandidat ključ koji je odabran da jedinstveno odredi n torku unutar relacije.

**4. Vanjski ili strani ključ** - atribut ili skup atributa unutar jedne relacije koji odgovara kandidat ključu neke (moguće i iste) relacije.
  
</details>

---
<br>
<br>

<details>
<summary><strong>11. Navedite i objasnite operacije u relacijskom modelu.</strong></summary>

<ins>**Tradicionalni operatori**</ins> izvode se na dvije relacije

**1. unija** - relacija koju čine sve n torke prve i druge relacije

**2. presjek** - relacija koju čine n torke zajedničke za obje relacije

**3. razlika** - relacija koju čine sve n torke koje se nalaze u prvoj, ali se ne nalaze u drugoj relaciji

**4. Kartezijev proizvod** - relacija koju čine sve moguće kombinacije parova n torki s tim da je prva n torka iz prve, a druga iz druge relacije. izvode se na dvije relacije.

<ins>**Izvedeni operatori**</ins>

**1. selekcija (ograničenje, restrikcija,izbor)** - rezultat su samo one n torke koje zadovoljavaju postavljene uvjete.

**2. projekcija** - rezultat je izbor određenih atributa polazne relacije

**3. spajanje** - iz dvije relacije stvara novu relaciju od svih kombinacija parova n torki koji zadovoljavaju postavljene uvjete

**4. dijeljenje** - kreira novu relaciju na temelju jedne binarne i jedne unarne relacije

</details>

---
<br>
<br>

<details>
<summary><strong>12. Što je modeliranje podataka i nacrtati faze modeliranja od stvarnog svijeta do baze podataka?</strong></summary>

**Modeliranje podataka (eng. data mining)** je tehnika organiziranja i dokumentiranja podataka sustava

<img width="189" height="375" alt="image" src="https://github.com/user-attachments/assets/31181aa4-c5ac-4c3c-9efa-85bbe2e49102" />

</details>

---
<br>
<br>

<details>
<summary><strong>13. Pojasniti preslikavanje iz ER modela u relacijski model.</strong></summary>

<ins>**VEZA JEDAN: VIŠE**</ins> - Primarni  ključ  entiteta  sa  strane  veze  JEDAN  doda  se  kao  strani  ključ  u  entitet  sa strane  veze VIŠE

<ins>**VEZA VIŠE : VIŠE**</ins> - Doda  se novi  entitet,  koji  sadrži primarne ključeve  obaju  rubnih  entiteta. Ti  atributi zajedno  tvore složeni primarni ključ  novonastalog  entiteta.

**Usporedne veze** - Svaku  vezu  zamijenimo  s  po  jednim  stranim  ključem  u  relaciji  na  strani  veze VIŠE  (usporedne  veze  se  preslikaju  u  jednu,  ali  s   uvođenjem  dodatnog  stranog ključa). Da  bi  razlikovali  veze  među  entitetima  stranim  ključevima  damo  različite nazive.

**Povratne veze** - Doda  se strani ključ  jednak primarnom ključu  relacije.  Za  povratne  veze  vrijedi  da  je   strani  ključ  jednak primarnom  ključu relacije,  ali pod  drugim imenom.

</details>

---
<br>
<br>

<details>
<summary><strong>14. Što su funkcijeske ovisnosti?</strong></summary>
  
**Funkcijska ovisnost** je odnos između atributa u relaciji u kojem vrijednost jednog atributa određuje vrijednost drugog atributa.

</details>

---
<br>
<br>

<details>
<summary><strong>15. Što su normalne forme i objasniti ih?</strong></summary>
  
**Normalna forma** je stupanj organizacije relacije u relacijskoj bazi podataka kojim se osigurava pravilna struktura podataka i smanjuje redundancija. Najčešće normalne forme su 1NF, 2NF i 3NF.

**1NF** – atributi imaju atomske vrijednosti, nema ponavljanja.

**2NF** – svi neključni atributi potpuno ovise o primarnom ključu.

**3NF** – nema tranzitivnih ovisnosti između neključnih atributa.

</details>

---
<br>
<br>

<details>
<summary><strong>16. U čemu je sličnost, a u čemu razlika između primarnog i jedinstvenog ključa?</strong></summary>

<ins>**Sličnost**</ins>

- I primarni ključ i jedinstveni ključ služe za jedinstveno identificiranje zapisa (n-torki) u tablici.

- Kod oba ključa vrijednosti se ne smiju ponavljati u stupcu ili skupu stupaca.

<ins>**Razlika**</ins>

**Primarni ključ** - u tablici može postojati samo jedan primarni ključ, ne smije imati NULL vrijednosti, glavni je identifikator zapisa.

**Jedinstveni ključ** - u tablici može postojati više jedinstvenih ključeva, može sadržavati NULL vrijednosti (ovisno o sustavu baze podataka), služi za dodatno osiguravanje jedinstvenosti podataka.

</details>

---
<br>
<br>

<details>
<summary><strong>17. Što se podrazumijeva pod Kartezijevim proizvodom? Navedite primjer.</strong></summary>

**Rezultat Kartezijevog produkta** dvije tablice je tablica koja se sastoji od svih mogućih kombinacija parova n torki, pri čemu je prva n torka iz prve, a druga iz druge tablice.

- NPR: Ako prva tablica ima 3 retka, a druga 2 retka, rezultat Kartezijevog proizvoda ima 3 × 2 = 6 redaka.

</details>

---
<br>
<br>

<details>
<summary><strong>18. Koji uvjeti moraju biti ispunjeni da bi se nad relacijskim tablicama mogli izvršiti operatori unije, presjeka i razlike?</strong></summary>
  
- Obje tablice moraju imati ista imena atributa a time i isti stupanj
  
- Svaki atribut jedne tablice se preslikava na odgovarajući (unijski kompatibilan) atribut druge tablice, tj. atributi s istim imenima su definirani nad istom domenom.

</details>

---
<br>
<br>

<details>
<summary><strong>19. O kojoj je funkcijskoj ovisnosti riječ kod treće normalne forme?</strong></summary>
  
**Tranzitivna funkcijska ovisnost** - neključni atribut ne smije biti funkcijski ovisan o drugom neključnom atributu, nego mora ovisiti isključivo o primarnom ključu.

</details>

---
<br>
<br>

<details>
<summary><strong>20. U čemu je razlika između DDL i DML naredbi SQL-a?</strong></summary>

**DDL** služi za definiranje i mijenjanje strukture baze podataka. (CREATE, ALTER, DROP)

**DML** služi za rad s podacima unutar tablica (INSERT, UPDATE, DELETE).

</details>

---
<br>
<br>

<details>
<summary><strong>21. Koji se postupci apstrakcije koriste u E-R modeliranju za formiranje entiteta, a koji za formiranje veza?</strong></summary>

<ins>**Formiranje Entiteta**</ins>

Generalizacija - Tipovi entiteta niže razine uopćuju se tipom entiteta više razine (nadtip i podtip). Opisuje se vezom “jest” (engl. is a).

<ins>**Formiranje Veza**</ins>

Agregacija - Formiranje novog pojma, višeg stupnja, na temelju odnosa postojećih pojmova.

</details>

---
<br>
<br>

<details>
<summary><strong>22. U čemu je razlika između operatora selekcije i projekcije? Navedite primjer.</strong></summary>
  
**Selekcija** kao rezultat daje točno određene ntorke (redove) iz tablice tj. samo one n-torke koje zadovoljavaju zadani kriterij.
- NPR: da bi se iz tablice "Dobavljači - D" izdvojili samo oni dobavljači koji se nalaze u Osijeku, koristi se operator ograničenja: D gdje je grad=‘Osijek‘
  
**Projekcija** kao rezultat daje tablicu koja se sastoji samo od određenih atributa (stupaca) zadane tablice

- NPR: ako se tablica dobavljača – D sastoji od slijedećih atributa: D(D#,Šifra,Naziv,Adresa,Mjesto), a žele se prikazati samo podaci o šifri i nazivu, koristi se projekcija.

</details>

---
<br>
<br>

<details>
<summary><strong>23. Koje uvjete mora zadovoljiti kandidat za primarni ključ?</strong></summary>
  
**1. jedinstvenost** - na relacijskoj shemi niti u jednom trenutku ne mogu postojati dvije n-torke s jednakim vrijednostima skupa atributa K. 

**2. minimalnost** - niti jedan pravi podskup od skupa atributa K nema svojstvo jednoznačnosti.

</details>
