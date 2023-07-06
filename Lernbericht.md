# Lernbericht

**Mitglieder:** Cyril Lutziger

## Einleitung
In diesem Projekr war es die Aufgabe, eine Website mithilfe von `HTML` und `CSS` zu erstellen. Ich habe mich dazu entschieden, eine Portfolio Webseite über mich zu machen, welches alle nötigen Informationen über mich beinhalten.

## Was habe ich gelernt?
In diesem Projekt, habe ich natürlich die sprache von `HTML` und `CSS` gelernt, aber besonders die Social bar auf der rechten Seite mit allen Links und auch Hover effekten. 
![Social-Links](https://github.com/Cikle/My-Portfolio/assets/110893288/b91e5812-27a3-48dd-ac56-76947cc54b73)



## Erklärung
Um eine Editor-Datei zu erstellen und Daten in diese Datei zu schreiben, wird in diesem Skript der Text des Berichts in eine Textdatei geschrieben und anschliessend mit dem Editor geöffnet. Hier ist der relevante Abschnitt des Skripts:

```ps1
# Define the editor name
$editorName = "SystemMetricsReport-" + (Get-Date -Format "yyyy-MM-dd-HH-mm-ss")

# Save the report to a file
$reportPath = Join-Path -Path $env:TEMP -ChildPath "$editorName.txt"
$systemMetricsReport | Out-File -FilePath $reportPath -Encoding UTF8

# Open the report in an editor
notepad.exe $reportPath
```

Zuerst wird der Name des Editors definiert. In diesem Fall wird der Name des Editors als "SystemMetricsReport-" und das aktuelle Datum und die Uhrzeit im Format "yyyy-MM-dd-HH-mm-ss" verwendet. Dieser Name wird verwendet, um die Editor-Datei zu benennen.

Der Bericht wird mit dem Befehl Out-File in die Textdatei geschrieben. Dabei wird der Dateipfad für die Datei mit Hilfe des Join-Path-Befehls erstellt. Hier wird das temporäre Verzeichnis des Benutzers ($env:TEMP) als Basispfad verwendet und der Editor-Name ($editorName) mit der Erweiterung ".txt" als Kindpfad hinzugefügt. Der Bericht wird mit UTF-8-Kodierung (-Encoding UTF8) in die Datei geschrieben.

Schliesslich wird der Befehl notepad.exe verwendet, um die Editor-Datei mit dem entsprechenden Dateipfad ($reportPath) zu öffnen. Der Editor, der standardmässig mit dem System verbunden ist (in diesem Fall Notepad), wird verwendet, um die Datei zu öffnen.

Durch diese Schritte wird der generierte Bericht in eine Editor-Datei geschrieben und anschliessend automatisch in Notepad oder einem anderen Standardeditor geöffnet.

## Verifikationen

* `Textbeschreibung:` Die Textbeschreibung dient zur Verständlichkeit des Codes.

* `Code:` Dieser Code ist ein Beispiel, wie man eine ForEach-Schleife benutzen könnte.

* `Bild:` Kein Bild vorhanden welches zur Veranschaulichung des Codes dienen würde.


## Reflexion zum Arbeitsprozess

👍Bei meiner Arbeit lief gut, dass ich sehr schnell voran gekommen bin.

👎Bei meiner Arbeit lief nicht gut, dass ich vielmals Fehler hatte, da ich nicht wusste wie ich mit dem Skript vorgehen musste.

VBV: Für mein nächstes Projekt nehme ich mir vor, alles besser vorauszuplanen, sowie das PAP früher zu erstellen.
