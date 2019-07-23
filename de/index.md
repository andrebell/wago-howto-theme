---
layout: page
title: WAGO HowTo Theme
lang: de
lang-ref: wago-howto-theme
redirect_from: '/'
---

# {{ page.title }}

Das WAGO HowTo Theme ist ein [Jekyll] theme für WAGO Repositories auf [GitHub], die [GitHubPages] zur Dokumentation nutzen möchten. Die [Dokumentation dieses Themes](https://andrebell.github.io/wago-howto-theme) erfolgt selber in [GitHubPages].

## Abhängigkeiten

Dieses Theme nutzt die standard [Jekyll] Installation auf [GitHubPages]. Als Plugins wird auf 

- [Jemoji] für Emojis und die Flaggen in der Sprachauswahl
- [JekyllRedirectFrom] für den Redirect auf die Defaultsprache in mehrsprachigen Seiten

zurückgegriffen.

## Schnellstart

1. Um dieses Theme in einem Repository zu nutzen muss eine `_config.yml` Datei im Basisverzeichnis für [GitHubPages] angelegt werden.

	```yaml
	title: Ein Titel für die Webseite
	author: Max Mustermann
	email: max.mustermann@wago.com
	remote_theme: andrebell/wago-howto-theme
	plugins:
	  - jemoji
	  - jekyll-redirect-from
	```

1. Innerhalb des Repositories muss es ein oder mehrere Markdown-Files geben. Beispielsweise dieses `index.md`:

	```markdown
	---
	layout: page
	title: Eine Indexseite
	lang: de
	lang-ref: index
	---
	# Eine Indexseite

	Hier kommt der Text...
	```

1. Innerhalb von [GitHub] muss für das Repository [GitHubPages] in den Einstellungen aktiviert werden.

## Nächste Schritte

Diese Dokumentation gibt weiterführende Infos in den folgenden Kapiteln:

- Markdown: Für die Nutzung dieses Themes müssen die Inhalte in Markdown geschrieben werden. In diesem Kapitel werden ein paar kurze Infos sowie Links bereitgestellt. Darüber hinaus werden ein paar Besonderheiten zum Markdown Prozessor Kramdown gegeben, der in GitHub Pages eingesetzt wird.
- Jekyll: In diesem Kapitel werden ein paar Grundlagen zu [Jekyll], dem Tool hinter [GitHubPages], sowie zu der in Jekyll verwendeten Template Engine Liquid gegeben.
- Verzeichnisse: Tipps zur Verzeichnisstruktur bei der Verwendung dieses Themes. 
- GitHub Pages: Hier gibt es eine kurze Anleitung, wie die Einstellungen auf GitHub durchgeführt werden.
- Internationalisierung: Soll die Dokumentation mehrsprachig ausgeführt werden, so beschreibt dieses Kapitel worauf es ankommt und wie das Theme das realisiert.
- Includes: Einige wiederkehrende Elemente können vereinfacht auf Seiten hinzugefügt werden. Die möglichen Includes dieses Themes werden hier erläutert.
- Konfiguration: Alle möglichen Konfigurationsparameter des Themes werden hier dargestellt.
- Versionshistorie

## Lizenz

Dieses Theme steht als Open Source unter der [MIT License] zur Verfügung.

[Jekyll]: https://jekyllrb.com/ "Jekyll"
[GitHub]: https://www.github.com/ "GitHub"
[GitHubPages]: https://help.github.com/en/articles/what-is-github-pages "GitHub Pages"
[MIT License]: https://opensource.org/licenses/MIT "MIT Lizenz"
[Jemoji]: https://github.com/jekyll/jemoji "Jemoji"
[JekyllRedirectFrom]: https://github.com/jekyll/jekyll-redirect-from "Jekyll-Redirect-From"
