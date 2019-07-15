---
layout: page
title: Includes des WAGO HowTo Themes
---
# {{ page.title }}
{:.no_toc}

- Inhaltverzeichnis
{:toc}

## howtoinfo.html

Auf einzelnen Schritt für Schritt Anleitungen kann eine Überblicksinfo zum Kontext, dem Schwierigkeitsgrad und dem Aufwand über das Include `howtoinfo` gegeben werden. Dies bindet man in seinem Markdown wie folgt ein:

```
{%- raw -%}
{% include howtoinfo.html
	compatibility = "Diese Anleitung nutzt als Basis den Controller 
		PFC200 in Firmware... (relevante Abhängigkeiten)"
	difficulty = 2
	effort = 4
%}
{% endraw %}
```
Das erscheint dann in der Ausgabe als:

{% include howtoinfo.html
	compatibility = "Diese Anleitung nutzt als Basis den Controller PFC200 in Firmware... (relevante Abhängigkeiten)"
	difficulty = 2
	effort = 4
%}

## info.html

Eine kurze Info kann über den Include `info.html` erzeugt werden. Beispiel:

```
{%- raw -%}
{% include info.html 
	content = "Dies ist eine kurze zusätzliche Info."
%}
{% endraw %}
```

Diese Info erscheint dann im HTML Output als:

{% include info.html 
	content = "Dies ist eine kurze zusätzliche Info."
%}

