# 📋 Tvorba Test Cases na základě dokumentace v Jira

V Jira jsem zpracovala požadavky z dodané dokumentace a rozdělila je podle jednotlivých oblastí do sprintů. V této ukázce prezentuji Sprint 1 – Přihlašování, bezpečnost a profil uživatele.
V Jira jsem vytvořila Stories, které obsahuje user story a akceptační kritéria, které byly uvedeny v dokumentaci.
<br>

## 🔍 Test Case 1

Jako první ukázku uvádím pozitivní test ověřující úspěšné přihlášení uživateleplatnými přihlašovacími údaji.
<br>

### 🧪 US-01: Přihlášení univerzitním e-mailem
<br>

#### User Story:

Jako student nebo vyučující, chci se do aplikace přihlašovat pomocí své univerzitní e-mailové adresy a hesla, abych získal přístup k rozvrhu laboratoří podle svých oprávnění.

#### Akceptační kritéria:

1. Přihlašovací obrazovka obsahuje pole „Univerzitní e-mail“, „Heslo“, tlačítko „Přihlásit se“ a odkaz „Zapomenuté heslo?“.
2. Při zadání nepovolené domény (např. běžný @gmail.com, pokud univerzita vyžaduje tvar @univerzita.cz) se zobrazí upozornění: „Použijte oficiální univerzitní e-mailovou adresu“.
3. Při zadání nesprávného hesla se zobrazí chybová zpráva: „Nesprávný e-mail nebo heslo“. Vyplněný e-mail zůstává zachován.
4. Po třech neúspěšných pokusech se tlačítko pro přihlášení dočasně zablokuje na 30 sekund.
5. Po úspěšném přihlášení se relace uloží na zařízení a uživatel je přesměrován na hlavní obrazovku katalogu.
<br>

### 🗂️ Ukázka položek Sprintu 1
![Položky sprintu 1](images/mals_sprint1.png)

Na základě user story a akceptačních kritérií jsem navrhla test cases, které jsem zpracovala pomocí nástroje QAlity Plus v Jira. U jednotlivých test cases jsem definovala předpoklady (preconditions), testovací kroky, testovací data a očekávané výsledky.

Test case jsem následně propojila s příslušnou user story, aby byla zachována dohledatelnost mezi požadavky a navrženými testy (traceability).
<br>

### 🔗 Připojené požadavky v  Jira k US-01: Přihlášení univerzitním e-mailem
![Připojené požadavky](images/mals26_pozadavky.png)
<br>
<br>

### 🧪 Test Cases v QAlity Plus k US-01: Přihlášení univerzitním e-mailem
<br>

Níže uvádím jako ukázku detail test case MALS-26: Ověřit přihlášení platnými přihlašovacími údaji.

<br>

![Test Case v QAlity Plus](images/mals26_qality.png)

<br>

![Test Case v QAlity Plus](images/mals26_qalitytest.png)

<br>
<br>


## 🔍 Test Case 2

Druhá ukázka je zaměřena na bezpečnostní chování aplikace po odhlášení uživatele. Ověřuje, že se uživatel po kliknutí na tlačítko "Zpět" po odhlášení nemůže vrátit zpět do účtu, ze kterého se odhlásil.
<br>

### 🧪 US-05: Bezpečné odhlášení z aplikace
<br>

#### User Story:

Jako uživatel, chci mít možnost se kdykoliv odhlásit ze svého profilu v nastavení aplikace, abych ochránil své rezervace při půjčení telefonu jiné osobě.

#### Akceptační kritéria:

1. Ve spodní části obrazovky profilu je umístěno tlačítko „Odhlásit se“.

2. Po stisknutí se zobrazí potvrzovací dialog: „Opravdu se chcete odhlásit?“.

3. Po potvrzení se přihlašovací klíče odstraní z lokální paměti zařízení.

4. Uživatel je přesměrován na přihlašovací obrazovku a systémové tlačítko „Zpět“ neumožní návrat do odhlášeného profilu

<br>

### 🔗 Připojené požadavky v  Jira k US-05: Bezpečné odhlášení z aplikace
![Připojené požadavky](images/mals05_pozadavky.png)
<br>
<br>

### 🧪 Test Cases v QAlity Plus k US-05: Bezpečné odhlášení z aplikace
<br>

Níže uvádím jako ukázku detail test case MALS-63: Ověřit znemožnění návratu do profilu tlačítkem "Zpět" po odhlášení

<br>

![Test Case v QAlity Plus](images/mals05a.png)

<br>

![Test Case v QAlity Plus](images/mals05b.png)



<br>




