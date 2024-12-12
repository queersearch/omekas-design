# omeka-s-design
Alle Dateien/Codes, die im Zuge der Frontendgestaltung erzeugt wurden

* Ordner **CSS** = enthält aktuelle CSS Datei (omekastyles.css) und Backups (omekastyles-Datum.css); momentan über CSS-Editor eingebunden: Lato (font): https://fonts.googleapis.com/css2?family=Lato:ital,wght@0,400;0,700;1,400&display=swap **Achtung:** Enthält Pfade zu Bilddateien
* Ordner **theme-erweiterungen** = enthält verschiedene Änderungen an Theme-Dateien, die beim Umzug von der Test- auf die Produktivinstanz angeglichen werden müssen
  * **volltextsuche.phtml** = Templaterweiterung, um auf der Homeseite eine Volltextsuche einbinden zu können. Pfad auf Omeka S Instanz: themes/foundation/view/commmon/block-template/
       **Achtung:** Enthält Pfad in Bilddatei sowie bei action=""; muss bei Umzug von Test- auf Produktivinstanz angeglichen werden
  * **theme.ini** = hier müssen Templatererweiterungen initialisiert werden. Pfad auf Omeka S Instanz: themes/foundation/config/
  * **resource-values.phtml** = Veränderungen am Code, um den einzelnen Datenfeldern unterschiedliche CSS-Klassen geben und sie dadurch per CSS formatieren (z. B. ausblenden, einfärben etc.) zu können. Liste der Veränderungen hier: https://github.com/queersearch/ptf-setup/issues/33#issuecomment-2438541759. Pfad auf Omeka S Instanz: themes/foundation/view/commmon/
  * **show.phtml** = Veränderungen am Code, um eine body-class zu erzeugen, die über CSS angesprochen werden kann. Außerdem Einfügung eines Code-Schnipsels, um die Möglichkeit zu realisieren, dass Nutzende sich recherchierte Objekte merken und sich deren Metadaten exportieren lassen können. Die Liste der Veränderungen findet sich hier: https://github.com/queersearch/ptf-setup/issues/33#issuecomment-2438541759. Pfad auf Omeka S Instanz: themes/foundation/view/omeka/site/item/
  * **browse.phtml** = Veränderungen am Code, um Filterfunktion der Landingpage nach Büchern, Zeitschriften etc. anzuwenden. Außerdem werden hier die Überschriften gebildet. Veränderungen sind Im Code ausgezeichnet. Pfad auf Omeka S Instanz: themes/foundation/view/omeka/site/item/
  * Ordner: **modules-aenderungen**
  * **previous-next.phtml** = Veränderungen am Code, um die Pfeile, mit denen man von einem zum nächsten Objekt navigieren kann, anzupassen und mit Text zu versehen; Pfad auf Omeka S Instanz: modules/BlockPlus/view/common/resource-page-block-layout/ **Achtung**: Hier muss noch herausgefunden werden, wie man die Änderungen nachhaltig gestalten kann, damit nicht beim nächsten Modul-Update alle Änderungen wieder überschrieben werden
