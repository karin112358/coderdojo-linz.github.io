---
layout: sushi
title: Scratch Fang-Mich
description: In diesem Spiel musst du versuchen, dem Haifisch zu entkommen.
---

# Scratch Fang-Mich

In diesem Spiel bist du ein Fisch, der dem großen Haifisch entkommen muss. Schaffst du es?

## Bühne und Figuren anlegen

1. ![Bühnenbild auswählen](scratch-fang-mich-v3/01-background.png){: .right}
Als erstes legst du fest, wie dein Spielfeld aussehen soll. Wir brauchen zuerst das Aquarium, in dem die Fische schwimmen. Wähle als erstes rechts unten unter *Bühnenbild wählen* ein Bühnenbild aus, zum Beispiel ein Underwater 1.

2. ![Figur löschen](scratch-fang-mich-v3/02-delete-scratchy.png){: .right}
Als nächstes lösche die Figur Scratchy mit dem Namen *Sprite 1* indem du mit der rechten Maustaste darauf klickst. 
Im angezeigten Menü kannst du Scratchy löschen.

3. ![Figuren hinzufügen](scratch-fang-mich/03-fish.png){: .right}
Jetzt brauchen wir einen Haifisch sowie einen Fisch, mit dem wir dem Haifisch entkommen wollen. Klicke dazu auf *Figur wählen* und füge einen Fisch sowie einen Haifisch dazu. Natürlich können es auch andere Figuren sein, zum Beispiel ein Käfer, der dem Vogel davonläuft oder eine Person die dem Löwen davon läuft.

4. ![Fisch gruppieren](scratch-fang-mich-v3/04-to-group.png){: .right}
Damit der kleine Fisch auch kleiner ist als der große Haifisch, müssen wir den Fisch verkleinern. Davor müssen wir ihn aber noch *gruppieren*, sodass im nächsten Schritt der ganze Fisch kleiner wird, nicht nur die Schwanzflosse. Wähle dazu den Fisch bei den Figuren aus, sodass er blau umrandet ist. Klicke anschließend auf den Tab *Kostüme*. Führe die Maus auf die karrierte Fläche und drücke die linke Maustaste. Halte diese gedrückt und bewege deine Maus nun so, dass sich der ganze Fisch innerhalb der grauen Linien befindet. Lass los und führe deine Maus nach oben, wo du rechts neben den beiden blauben Pfeilen ein Symbol siehst. Drücke darauf und der Fisch ist nun gruppiert.

5. ![Fisch verkleinern](scratch-fang-mich-v3/05-resize.png){: .right}
Damit der kleine Fisch auch kleiner ist als der große Haifisch, müssen wir den Fisch verkleinern. Wähle dazu den Fisch bei den Figuren aus, sodass er blau umrandet ist. Klicke anschließend auf den Tab *Kostüme*, wähle den Fisch aus und verkleinere ihn, indem du ihn an den Ecken kleiner ziehst.

6. ![Drehpunkt setzen](scratch-fang-mich-v3/06-fish-center.png){: .right}
Damit der kleine Fisch sich auch um den richtigen Punkt dreht, wenn er umdreht, musst du den Drehpunkt des Kostüms anpassen. Wähle dazu den Fisch bei den Figuren aus, sodass er blau umrandet ist. Klicke anschließend auf den Tab *Kostüme*, wähle den Fisch aus und klicke auf das Kreuz-Bildchen im rechten oberen Eck. Das angezeigte Kreuz soll genau über der Mitte des Fisches sein.

7. ![Figuren benennen](scratch-fang-mich-v3/07-rename.png){: .right}
Damit du später die Figuren leichter verwenden kannst, gib ihnen Namen wie *Haifisch* und *Fisch*. Du kannst die Eigenschaften von Figuren ändern, indem du auf das blaue *i* links über der Figur klickst.

## Fisch bewegen

1. ![Fisch bewegen](scratch-fang-mich-v3/08-move-fish.png){: .right}
Damit du den Fisch bewegen kannst, musst er nach links und rechts sowie oben und unten bewegt werden können.<br/><br/>
  • Wähle zuerst den Fisch aus, damit er blau umrandet ist.<br/>
  • Im Tab *Code* kannst du deinen Fisch nun bewegen. Verwende das Ereignis *Wenn Taste ... gedrückt* unter *Ereignisse*.<br/>
  • Verknüpfe es jeweils mit einer Drehung *setze Richtung auf ...* unter *Bewegung*, damit der Fisch in die richtige Richtung schaut.<br/>
  • Außerdem brauchen wir *gehe ...er Schritt*, um den Fisch zu bewegen.<br/><br/>
Für *Pfeil nach oben* gedrückt: Richtung 0 Grad, gehe 10er-Schritte.<br/>
Für *Pfeil nach unten* gedrückt: Richtung 180 Grad, gehe 10er-Schritte.<br/>
Für *Pfeil nach rechts* gedrückt: Richtung 90 Grad, gehe 10er-Schritte.<br/>
Für *Pfeil nach links* gedrückt: Richtung -90 Grad, gehe 10er-Schritte.<br/><br/>
Je größer die Schrittanzahl, desto schneller ist dein Fisch.


## Haifisch bewegen

1. ![Haifisch bewegen](scratch-fang-mich-v3/09-move-shark.png){: .right}
Jetzt soll der Haifisch im Aquarium herumschwimmen.<br/><br/> 
  • Wähle dazu den Haifisch aus, damit er blau umrandet ist.<br/>
  • Im Tab *Code* kannst du den Haifisch nun bewegen.<br/>
  • Unter *Ereignisse* wähle *Wenn ... angeklickt*.<br/>
  • Anschließend wähle *wiederhole fortlaufend* bei *Steuerung* aus.<br/>
  • Bewege den Haifisch mit *gehe 10er-Schritt*, *warte 0,1 Sek.", *pralle vom Rand ab* und *drehe dich um ... Grad*<br/>
  • Um etwas mehr Zufall reinzubringen, nimm im Menü *Operatoren* den Block *Zufallszahl von 1 bis 10* und ziehe ihn an die Stelle der 15 Grad.

  
## Fisch fangen

1. ![Fisch wird berührt](scratch-fang-mich-v3/10-touch-fish.png){: .right}
Wenn der Haifisch den Fisch berüht, soll der Fisch ausgeblendet und wieder ins linke obere Eck gesetzt werden.<br/><br/> 
  • Wähle dazu den Fisch aus, damit er blau umrandet ist.<br/>
  • Im Tab *Code* kannst du den Fisch verschwinden lassen, sobald er den Haifisch berührt.<br/>
  • Unter *Ereignisse* wähle *Wenn ... angeklickt*.<br/>
  • Setze den Fisch an Position -230 und 170 mittels *gehe zu x: -230, y: 170*, um den Fisch ins linke obere Eck zu setzen, und *zeige dich*.<br/>
  • Falls jetzt der Hai berührt wird (*Steuerung* *falls ... dann*), dann *sende "berührt" an alle*, *verstecke dich*, *warte 5 Sekunden*, *zeige dich*, und gehe wieder ins linke obere Eck mit *gehe zu x: -230, y: 170*. Anschließend sage *Willkommen zurück* für 2 Sekunden.


2. ![Hai wird berührt](scratch-fang-mich-v3/11-touch-shark.png){: .right}
Wenn der Haifisch den Fisch berüht, soll er zwei mal schnappen und das Spiel "Game Over" sein.<br/><br/> 
  • Wähle dazu den Haifisch aus, damit er blau umrandet ist.<br/>
  • Im Tab *Code* kannst du den Haifisch "Game Over" sagen lassen.<br/>
  • Unter *Ereignisse* wähle *Wenn ich ... empfange*, der Hai reagiert somit auf die vom Fisch ausgelöste Nachricht.<br/>
  • Anschließend wähle *wiederhole 2 mal* bei *Steuerung* aus.<br/>
  • Um den Haifisch schnappen zu lassen, gibt es unter *Aussehen* verschiedene Varianten des Hais. Füge folgende Blöcke in den Wiederhol-Block: *wechsle zu Kostüm b*, *warte 0,3 Sek.*, *wechsel zu Kostüm a*, *warte 0,3 Sek.*<br/>
  • Und um den Haifisch "Game over" sagen zu lassen, füge einen neuen *Wenn ich ... empfange* Block hinzu und *sage "Game Over!" für 4.5 Sekunden*.

## Weitere Ideen

* Mach das Spiel schwieriger, indem du einen zweiten, langsameren Haifisch dazu gibst.
* Baue einen Uhr ein um zu sehen, wie lange du dem Haifisch entkommen kannst.
* Steuere den Fisch mit der Maus anstatt der Tastatur.


## Ausprobieren

Du kannst das fertige Projekt unter [https://scratch.mit.edu/projects/72919318/](https://scratch.mit.edu/projects/72919318/){:target="_blank"} ausprobieren.