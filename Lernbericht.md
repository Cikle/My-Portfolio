# Lernbericht

**Mitglieder:** Cyril Lutziger

## Einleitung
In diesem Projekr war es die Aufgabe, eine Website mithilfe von `HTML` und `CSS` zu erstellen. Ich habe mich dazu entschieden, eine Portfolio Webseite über mich zu machen, welches alle nötigen Informationen über mich beinhalten.

## Was habe ich gelernt?
In diesem Projekt, habe ich natürlich die sprache von `HTML` und `CSS` gelernt, aber besonders die Social bar auf der rechten Seite mit allen Links und auch Hover effekten. 


![Social-Links](https://github.com/Cikle/My-Portfolio/assets/110893288/b91e5812-27a3-48dd-ac56-76947cc54b73)



## Erklärung

Um die Social-Bar zu erstellen, musste ich einige CSS-Regeln hinzufügen und die entsprechenden Bilddateien für die Symbole verwenden. 

zuerst musste ich die Bilddateien für die Social-Media-Symbole (z.B. Discord.png, Instagram.png, Github.png) in den gleichen Ordner wie Ihre HTML-Datei hineinfügen.

Dannach fügte ich die folgenden CSS-Regeln in Ihre styles.css-Datei ein oder eine alternative wäre auch diese in den <style>-Bereich innerhalb des <head>-Tags Ihrer HTML-Datei einfügen:

```css
@import url("https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.3/css/all.min.css");

.social-links {
    position: fixed;
    top: 50%;
    right: 1.75%;
    transform: translateY(-50%);
    display: flex;
    flex-direction: column;
    align-items: center;
    z-index: 999;
}

.social-links a {
    display: block;
    margin-bottom: 30px;
}

.social-links img {
    width: auto;
    height: 1.55vh;
    opacity: 0.5;
    transition: all 0.3s ease-in-out, opacity 0.3s ease-in-out;
}

.social-links img:hover {
    transform: scale(1.2);
    opacity: 1;
    filter: drop-shadow(0 0 10px rgba(255, 255, 255, 0.5));
}
```

Dannach fügte ich den folgenden HTML-Code an der gewünschten Stelle in dem <body>-Tag ein:

```html
<div class="social-links">
    <a href="https://discord.com/users/507213791889588235" target="_blank"><img src="Discord.png" alt="Discord"></a>
    <a href="https://www.instagram.com/_cikle/" target="_blank"><img src="Instagram.png" alt="Instagram"></a>
    <a href="https://github.com/Cikle" target="_blank"><img src="Github.png" alt="Github"></a>
</div>
```

Und natürlich musste ich noch sicher stellen, dass die Pfade zu den Bilddateien in ```<img src="...">``` den tatsächlichen Dateinamen und Pfaden entsprechen.

Nachdem Speichern der HTML-Datei | CSS-Date und der öffnung im Webbrowser, sollte die Social-Bar auf der rechten Seite des Bildschirms angezeigt werden, und die Symbole werden beim Hover vergrößert und erhalten einen Schatten. Wenn Sie auf eines der Symbole klicken, öffnet sich die entsprechende Social-Media-Seite in einem neuen Tab.


## Verifikationen

* `Textbeschreibung:` Die Textbeschreibung dient zur Verständlichkeit des Codes.

* `Code:` Dieser Code ist ein Beispiel, wie man eine Social-Bar kriieren könnte.

* `Bild:` Bilder sind vorhanden welches zur Veranschaulichung des Codes dienen.


## Reflexion zum Arbeitsprozess

👍Bei meiner Arbeit lief gut, dass ich sehr schnell fertig geworden bin.

👎Bei meiner Arbeit lief nicht gut, dass ich viele verschiedene Mockups wie etwa 5 Websites kriiert habe, welche mir zum schluss gar nicht gefallen haben, und somit immer wieder neue kriierte bis zu dem hier.

VBV: Online nach design ideen nachzuschauen, ein gutes Mockup machgen, darüber nachdenken, und die Website einfach anfangen zu machen und auch zuende führen.
