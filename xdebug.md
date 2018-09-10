# Xdebug

> https://xdebug.org/

## Installation

Xdebug Extension herunterladen von [Xdebug Download](https://xdebug.org/download.php). Dabei auf die passende Version
achten (PHP Version, TS (Thread Safe oder nicht) und VC-Version). Die heruntergeladene dll in das ext-Verzeichnis kopieren und 
in der ````php.ini```-Datei aktivieren (Dateinamen natürlich anpassen oder Datei umbenennen:

    [Xdebug]
    zend_extension = php_xdebug.dll
	  xdebug.remote_enable = 1

## PhpStorm

### Variante A

1. In Webstorm eine Run-Konfiguration anlegen:

      * Typ: Web Application
      * Als Server den Server einrichten (Adresse und Port angeben, Xdebug auswählen)

2. Web-Server starten und in WebStorm auf Debug-Symbol clicken, Haltepunkte setzen und voilá!

### Variante B (Zeroconf)

1. Bookmarklet oder Browser-Extension installieren (https://confluence.jetbrains.com/display/PhpStorm/Browser+Debugging+Extensions).
Die Bookmarklets funktionieren natürlich auch in den anderen Browsern. Alternativ kann man einfach an die URL 
den Querystring ```?XDEBUG_SESSION_START=PHPSTORM``` anhängen

2. In PhpStorm auf den Telefonhörer clicken, Seite im Browser anfordern und voilá.

### Variante C: Remote debugging

Universal-Variante. Wichtigstes ist hierbei das Path-Mapping: Wo sind die Files bei mir lokal? Ansonsten muss zum
Start der Debug-Session der in PhpStorm gewählte Session-Name im Request "erscheinen".

## Links

* [Homepage](https://xdebug.org/)
* [How to use](https://deliciousbrains.com/xdebug-advanced-php-debugging/)
* [Sitepoint Article](https://www.sitepoint.com/getting-know-love-xdebug/)
* [Profiling](https://xdebug.org/docs/profiler)
* [Code Coverage](https://derickrethans.nl/code-coverage.html)


