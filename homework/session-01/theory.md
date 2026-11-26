# Teil 1: Theorie

Antworte kurz in eigenen Worten. Ergänze unter jeder Frage deine Antwort.

1. Du gibst die Adresse einer Webseite im Browser ein. Beschreibe die Aufgaben von Client und Server und nenne zwei Schritte, bis du die Seite siehst.

   **Antwort: der browser sucht im DNS die IP die zu dem Server passt, dann fragt er den Verbindungsaufbau an, mittels 3-Way-Handshake. Wenn die verbindung sicher ist, dann fragt der client(browser) die html seite an**

2. Was enthält eine HTTP-Anfrage ungefähr, und was kommt in der HTTP-Antwort zurück? Erkläre an einem einfachen Beispiel, was `GET` und ein Statuscode wie `200` bedeuten.

   **Antwort: HTTP-Version, Method, body und session cookie. get:eine methode die keinen http body besitzt und nützliche informationen mit query und params in der uli speichert. 200: ein statuscodes, der als antwort vom server kommt. er heißt succses oder "die daten sind angekommen.**

3. Wozu dienen `<!doctype html>`, `html`, `head` und `body` in einem HTML5-Dokument? Wo stehen der Seitentitel für den Browser-Tab und der sichtbare Haupttext?

   **Antwort: Doctype sagt, dass es ein HTML-Dokument ist. <html lang="de" ist die wurzel dann <head> gibt unsichtbare meta informationen. <body> beinhaltet text, bilder links**

4. Lies `<a href="/kurs" class="hinweis">Zum Kurs</a>`. Was ist das HTML-Element, was sind seine Attribute und was ist der sichtbare Text? Erkläre den Unterschied zwischen Element und Attribut.

   **Antwort: a steht für anker und ist das element, es hat das href und class atrebut.der sichtbare text ist Zum Kurs dahinter befindet sich der link.**

5. Eine Webseite soll Inhalt anzeigen, gestaltet sein und auf einen Klick reagieren. Welche Aufgaben übernehmen HTML, CSS und JavaScript jeweils? Nenne für jede Sprache ein kleines Beispiel.

   **Antwort: html ist für text, bilder und co zuständig, CSS für das Design und javascipt für die dynamische interaktion mit der Seite**

6. Lies diesen Ausschnitt. Was bewirken `action`, `method`, `type` und `name`? Welcher Wert wird beim Absenden unter welchem Namen übertragen?

   ```html
   <form action="/anmelden" method="post">
     <input type="email" name="kontakt" />
     <button type="submit">Senden</button>
   </form>
   ```

   **Antwort: action ist die action, die ausgeführt wird wenn dass Formular ausgeführt wird. method ist entweder post oder get jenach welche daten gesendet werden, post schickt über htlm body und get über query und params in der url.type ist der type des inputs(text ist text password ist {/_/_} email ist a@b.c. und submut ist abschicken) name ist der tag für labels und co.**

7. Erkläre, welche Elemente die Selektoren `p`, `#info`, `.hinweis` und `nav a` in diesem Beispiel auswählen. Kann ein Element von mehreren Regeln gleichzeitig betroffen sein?

   ```html
   <nav><a class="hinweis" href="#info">Info</a></nav>
   <p id="info" class="hinweis">Treffpunkt: Bibliothek</p>
   ```

   **Antwort:**

8. Eine Karte hat einen Rahmen. Wo liegen `padding` und `margin` relativ zu Inhalt und Rahmen? Welcher Wert vergrößert den Abstand **innerhalb** der Karte?

   **Antwort:**

9. Für `<p id="meldung" class="hinweis">Hallo</p>` gelten diese Regeln. Welche Textfarbe gewinnt und warum?

   ```css
   p {
     color: blue;
   }
   .hinweis {
     color: green;
   }
   #meldung {
     color: red;
   }
   ```

   **Antwort:**

## Teil 4: Reflexion

- Was war leicht?
- Was war schwierig?
- Welche Konzepte möchtest du in der nächsten Sitzung noch einmal erklärt bekommen?
- Hast du die Aufgaben selbstständig gelöst oder externe Quellen verwendet? Falls ja, welche?

**Meine Antworten:**
