Hausaufgabe 7

# Aufgabe 1

Welche verschiedenen Layout-Arten gibt es? Was sind die Unterschiede?
1. Festes Layout
   - Dimensionen fest in Pixeln angegeben, dynamische Anpassung nicht möglich
2. Flüssiges Layout
   - definiert in % des Viewports, wenn Viewport verändert -> Objekt skaliert, Inhalte bleiben in ihrer Größe erhalten
3. Elastisches Layout
   - Breitangaben in "em" (bezieht sich auf Schriftgröße). Layout skaliert mit Schriftgröße, nicht mit Bildschirmgröße
4. Adaptives Layout
   - festes Layout mit verschiedenen Versionen. Es gibt Breakpoints, an denen andere Styles gelten
5. Responsive Layout
   - Verbindung aus adaptiven und flüssigen Layout. Verfügt über Umbruchstellen und zwischen Umbruchstellen ist das Layout flüssig

Worauf beziehen sich Prozentangaben? Finden Sie heraus, worauf sich Prozentangaben bei
margin-left, margin-top, height, font-size und border-top-width beziehen.

Sie beziehen sich auf den Viewport. 50% bedeutet also die Hälfte des Viewports.

Was ist die Einheit em und was ist der Unterschied zur Einheit rem?
- EM: Vertikale Größe der Schrift, relativ zur Schriftgröße des Eltern-Elements. Über den Daumen gepeilt kann 1em als 16 Pixel gerechnet werden.
- REM: font-size wird immer relativ zum HTML-Element berechnet

Was bedeuten die Einheiten vw und vh?
Viewport width, Viewport height

# Aufgabe 2.1

Wieso ist es hilfreich dieses Rastersystem zu verwenden?
- Man muss nicht für jedes Element eine neue Klasse machen um die Breit zu bestimmen

Was passiert bei dem Rastersystem, wenn die HTML-Elemente genau auf 100% Breite
verteilt sind und der Rand eines Elements auf eine Größe von 3px gesetzt wird? (z.B. beim
<main>-Block im zweispaltigen Layout) Wie können Sie das Problem lösen?
- style="border:2px solid black;" sehe da kein Problem

Was bewirkt der CSS-Deklarationsblock [class*="col-"]{ float: left }?
- Alle mit col- deklarierten Klassen floaten left

Was bewirkt der komplette CSS-Deklarationsblock .row::after{ ... }? Öffnen
Sie die Seite in einem separaten Browsertab und zeigen Sie die Veränderung durch diese
CSS-Anweisung in den Entwicklertools von Chrome.
- 
