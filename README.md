# WRO_Future_Engineers_Xenoplex2

##Programmierung:
Auf unserem Roboter haben wir einen Arduino Mega verbaut. Mit diesem Controller steuern wir den gesamten Roboter. Programmiert wird er normalerweise über die Arduino IDE mit C++. Mit den seitlichen Ultraschallsensoren tastet sich der Roboter um das innere Viereck. Wenn der Ultraschallwert größer oder kleiner ist, lenkt der Roboter dementsprechend ein. Wenn der Wert größer als 230 ist, lenkt der Roboter stark ein, bis der Wert wieder unter 100 ist. Er geht aber erst in die Schleife, wenn eine Variable auf 0 gesetzt ist. Die Variable wird auf 0 gesetzt, wenn der Ultraschallwert kleiner als 100 ist, was bedeutet, dass der Roboter in der Nähe der Innenwand ist. Somit verhindern wir, dass er zu der Variable, welche die Kurven addiert, mehrere Werte addiert. Wenn der Wert 12 ist, fährt er noch eine Kurve und hält danach an. Mit der Programmierung der Pixi Kamera sind wir noch weit fortgeschritten, da wir zuvor noch nie etwas mit einer Pixi zu tun hatten.
Mit unseren zwei Starttastern können wir die zwei Unterprogramme starten, je nachdem, in welche Richtung der Roboter fahren soll.

##Motorisierung:
Als Antriebsmotor verwenden wir einen schwarzen Motor von fischertechnik. Für die Lenkung kommt ein Servo zum Einsatz. Eine H-Brücke sorgt als Motortreiber für den Antriebsmotor.

##Akku:
Als Akku verwenden wir einen 3-zelligen 12-Volt-Akku mit 37 Wh. Der Akku ist eine Eigenanfertigung.

##Hindernisumfahrung:
Für die Hinderniserkennung nutzen wir eine Pixi-Kamera, die über den I2C-Bus des Arduino kommuniziert. Die Pixi-Kamera gibt die Werte zwischen 0 und 2 aus: 0 bedeutet kein Hindernis erkennbar, 1 bedeutet rotes Hindernis erkennbar und 2 bedeutet grünes Hindernis erkennbar.
