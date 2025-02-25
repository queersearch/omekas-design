# omeka-s-design
Alle Dateien/Codes, die im Zuge der Frontendgestaltung erzeugt wurden

* Ordner **CSS** = enthält aktuelle CSS Datei (omekastyles.css) und Backups (omekastyles-Datum.css); momentan über CSS-Editor eingebunden: Lato (font): https://fonts.googleapis.com/css2?family=Lato:ital,wght@0,400;0,700;1,400&display=swap 
* Ordner **theme-erweiterungen** = enthält verschiedene Änderungen an Theme-Dateien, die beim Umzug von der Test- auf die Produktivinstanz angeglichen werden müssen
  * ~~**volltextsuche.phtml** = Templaterweiterung, um auf der Homeseite eine Volltextsuche einbinden zu können. Pfad auf Omeka S Instanz: **themes/foundation/view/commmon/block-template/**
       **Achtung:** Enthält Pfad in Bilddatei sowie bei action=""; muss bei Umzug von Test- auf Produktivinstanz angeglichen werden~~
  * ~~**theme.ini** = hier müssen Templatererweiterungen initialisiert werden. Pfad auf Omeka S Instanz: themes/foundation/config/~~
  * **resource-values.phtml** = Veränderungen am Code, um den einzelnen Datenfeldern unterschiedliche CSS-Klassen geben und sie dadurch per CSS formatieren (z. B. ausblenden, einfärben etc.) zu können. Liste der Veränderungen hier: https://github.com/queersearch/ptf-setup/issues/33#issuecomment-2438541759. Pfad auf Omeka S Instanz: **themes/foundation/view/commmon/**
  * **show.phtml** = Veränderungen am Code, um eine body-class zu erzeugen, die über CSS angesprochen werden kann (siehe: https://github.com/queersearch/ptf-setup/issues/33#issuecomment-2438541759). Außerdem Einfügung eines Code-Schnipsels, um die Möglichkeit zu realisieren, dass Nutzende sich recherchierte Objekte merken und sich deren Metadaten exportieren lassen können. Vor- und Zurück-Pfeile eingefügt, um zum vorigen bzw. nächsten Objekt einer Suchliste navigieren zu können (siehe auch unten previous-next.phtml), sowie einen Link zurück zur Liste der Suchergebnisse. Layout angepasst, um zwei Spalten zu haben (die beiden Spalten werden dann im CSS näher definiert). Pfad auf Omeka S Instanz: **themes/foundation/view/omeka/site/item/**
EDIT 23.02.2025: Vor- und Zurück-Pfeile auskommentiert;
  * **browse.phtml** = Veränderungen am Code, um Filterfunktion der Landingpage nach Büchern, Zeitschriften etc. anzuwenden. Hier ist auch eine Abfrage integriert worden, die die Objekte als Liste oder als Grid darstellt, je nachdem, ob es sich im eine Sammlung mit Bilder oder ohne handelt (die Abgrafe erfolgt über die ID der Sammlung). Veränderungen sind Im Code ausgezeichnet. Pfad auf Omeka S Instanz: **themes/foundation/view/omeka/site/item/**
* Ordner: **modules-aenderungen**
  * **previous-next.phtml** = Veränderungen am Code, um die Vor- bzw. Zurück-Pfeile auszukommentieren; diese werden über die Designvorlage (show.phtml) ins Template geschrieben und sollen nicht doppelt auftauchen (siehe oben).
  * **Module.php** = Veränderungen am Code, um bei Metadatabrowse einen anderen Text als den üblichen auszugeben; Pfad auf Omeka S Instanz: modules/MetadateBrowse/ **Achtung**: Kein besonders gelungeber Hack;
  * **linked-resources-by-item-set.phtml** = ist zuständig für den Teil, der die verknüpften Ressourcen wiedergibt; Übersetzungen händisch eingegeben; Pfad auf Omeka S Instanz: modules/BlockPlus/view/common/
  * **facet-select-range.phtml** = Übersetzungen händisch eingegeben; Pfad auf Omeka S Instanz: modules/AdvancedSearch/view/search/

