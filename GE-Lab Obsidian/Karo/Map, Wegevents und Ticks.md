- Wegpunkte auf Splines (von Robin gesetzt)
- mit jedem Wegpunkt, der passiert wird, wird der Tickcounter erhöht --> tickCounter++
	- TESTEN, OB TRANSFORMS, LEERE OBJEKTE/CUBES, TRIGGERBOXEN FUNKTIONIEREN
	- extra Triggerbox, um die Wegpunkte zu registrieren --> siehe Bild ![[WhatsApp Bild 2024-10-09 um 11.24.51_333496ab.jpg]]
- Wegevents (d.h. Personen stehen am Wegrand --> geben Quest, Dialog oder Kampf) werden beim Übertritt auf einen neuen Mapabschnitt, nach einer Rast und nach einem Kampf neu generiert und gespawnt
	- bei diesen Übergängen immer Schwarzblende
- feste Wegpunkt auf Map, die immer nach x Mapabschnitten angefahren werden
	- Startabschnitt
	- Ende
	- Unterwegs?

- 24 Ticks = 1 Tag
	- 12 Ticks Tag
	- 12 Ticks Nacht
	- Tickcounter immer hochzählen und entsprechend %12 Tag/Nacht setzen
	- Sonne macht Robin
	- Kämpfe dauern AnzahlRunden/2 Ticks
		- Runde = jeder Charakter und jeder Gegner greift einmal an/agiert

- sobald Mapstück betreten wird, werden zwei anschließende Map-Stücke geladen und vorherige Map-Stücke werden inaktiv gesetzt/gelöscht
	- Löschen ist aber erstmal Nice-To-Have, wichtiger ist der Ladevorgang
	- kontrollierte Zufälligkeit nur, wenn es nicht zu lange dauert



