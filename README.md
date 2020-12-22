# 4207_SimpleService

## Aufgabe:
Erstelle einen Task, dem ein int-Parameter übergeben werden kann

### Task:
- Die Aufgabe des Tasks ist das Zählen bis zu diesem Wert, wobei bei jeder Iteration 10ms gewartet werden muss
- Über `updateMessage()` wird ein String übergeben - je nach "Fortschritt" des Tasks. Dieser ist am Button als Text anzuzeigen
  - "Counting"
  - "READY"
- Während des Zählvorgangs ist der Fortschritt über `updateProgress()` zu aktualisieren

### Service
- Der Task ist in einem Service zu kapseln, welcher sofort bei Anwendungsbeginn startet
- Sobald der Service fertig ist, kann er durch Klick auf den Button erneut gestartet werden

### GUI / Bindings
- Binde folgende Properties des Buttons an den Fortschritt des Services
  - `opacityProperty` - Fortschritt 0 -> unsichtbar, Fortschritt Maximal -> sichtbar
  - `scaleXProperty` - multipliziere den Wert mit 5 für einen größeren Button
  - `scaleYProperty` - multipliziere den Wert mit 5 für einen größeren Button
  - `textProperty` - ändere den Text über `updateProgress()`


