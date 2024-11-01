# omeka-s-design
Alle Dateien/Codes, die im Zuge der Frontendgestaltung erzeugt wurden

* Ordner **CSS** = enthält aktuelle CSS Datei (omekastyles.css) und Backups (omekastyles-Datum.css)
* Ordenr **theme-erweiterungen** = enthält verschiedene Änderungen an Theme-Dateien
  * **volltextsuche.phtml** = Templaterweiterung, um auf der Homeseite eine Volltextsuche einbinden zu können. Pfad auf Omeka S Instanz: themes/foundation/view/commmon/block-template/ /
    **Achtung:** Enthält Pfad zu Bilddatei, muss bei Umzug von Test- auf Produktivinstanz angeglichen werden
  * **theme.ini** = hier müssen Templatererweiterungen initialisiert werden. Pfad auf Omeka S Instanz: themes/foundation/config/
  * **resource-values.phtml** = Veränderungen am Code, um den einzelnen Datenfeldern unterschiedliche CSS-Klassen geben und sie dadurch per CSS formatieren (z. B. ausblenden, einfärben etc.) zu können. Liste der Veränderungen hier: https://github.com/queersearch/ptf-setup/issues/33#issuecomment-2438541759. Pfad auf Omeka S Instanz: themes/foundation/view/commmon/
  * **show.phtml** = Veränderungen am Code, um eine body-class zu erzeugen, die über CSS angesprochen werden kann. Liste der Veränderungen hier: https://github.com/queersearch/ptf-setup/issues/33#issuecomment-2438541759. Pfad auf Omeka S Instanz: themes/foundation/view/omeka/site/item/
