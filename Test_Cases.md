# 📋 Tvorba Test Cases na základě dokumentace v Jira
<br>
V Jira jsem zpracovala veškeré požadavky z dokumentace a rozdělila si je podle oblastí do jednotlivých sprintů. V ukázce budu poožívat Sprint 1 - Přihlášení, bezpečnost a profil uživatele.
V Jira jsem vytvořila Story, které obsahuje User Story a Acceptance Criteria, které byly uvedeny v dokumentaci.
<br>

## 🔍 Test Cases


### 📝 US-01: Přihlášení univerzitním e-mailem
<br>

#### User story:

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

Na základě User Story a Acceptance Criteria jsem navrhla test cases, které jsem zpracovala pomocí nástroje QAlity Plus v Jira. U jednotlivých test cases jsem definovala preconditions, testovací kroky, testovací data a očekávané výsledky.

Test cases jsem následně propojila s příslušnou User Story, aby byla zachována dohledatelnost mezi požadavky a navrženými testy (traceability).
<br>

### 🔗 Připojené požadavky v  Jira k US-01: Přihlášení univerzitním e-mailem
![Připojené požadavky](images/mals26_pozadavky.png)
<br>
<br>

### Test Cases v QAlity Plus k US-01: Přihlášení univerzitním e-mailem
<br>

![Test Case v QAlity Plus](images/mals26_qality.png)

<br>

![Test Case v QAlity Plus](images/mals26_qalitytest.png)

<br>





