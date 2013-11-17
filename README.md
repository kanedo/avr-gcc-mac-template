avr-gcc-mac-template
====================

AVR-Project template for mac

installation
------------

[Crosspack](http://www.obdev.at/products/crosspack) in gewünschter Version installieren.
RWTH PSP Studenten nutzen Version `CrossPack-AVR-20100115.dmg`: 
```
	Based on WinAVR 20100110.
```

Als nächstes erweitert man seine `$PATH` Variable um `/usr/local/CrossPack-AVR/bin`

Wichtig jetzt das Template. Das gehört in den Ordner `/usr/local/CrossPack-AVR-20100115/etc/templates`

Makefile
--------
Das Makefile ist so geschrieben, dass es automatisch alle `*.c` Dateien mitkompiliert. Als C-Dialekt wird `gnu99` verwendet.
Angepasst werden müssen folgende Variablen:
```
DEVICE     = atmega644 
CLOCK      = 20000
```

To-Do
-----

Der Debugger ist ungetestet. Ich nutze es nur um meine Versuche zu bauen und auf warnings zu kontrollieren.