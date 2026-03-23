# Projektdokumentation

## 1. Einleitung

Die folgende Projektdokumentation beschreibt die Planung und Durchführung eines Projekts im Rahmen des Lernfeldes LF12a „Kundenspezifische Anwendungsentwicklung durchführen“, das der Autor im Rahmen seiner Umschulung zum Fachinformatiker für Anwendungsentwicklung bearbeitet.

Die Umschulung erfolgt bei der GFN in München. Ein konkreter Ausbildungsbetrieb ist zum jetzigen Zeitpunkt noch nicht bekannt, da es sich hierbei um ein schulisches Projekt im Rahmen des Unterrichts handelt.

Die Umschulung wird durch die Agentur für Arbeit gefördert und dient der beruflichen Neuorientierung von Personen, die in ihrem ursprünglich erlernten oder ausgeübten Berufsfeld auf Schwierigkeiten stoßen und sich neue berufliche Perspektiven erschließen möchten.

## 1.1 Projektbeschreibung

Im Rahmen des Projekts wird eine interne Webanwendung zur Verwaltung, Ausleihe und Nachverfolgung von Laborwerkzeugen konzipiert und entwickelt.

Die Projektidee entstand aus einem realen organisatorischen Problem in einem Laborumfeld. Dort werden verschiedene Werkzeuge von mehreren Mitarbeitenden gemeinsam genutzt. Im Austausch mit dem fachlichen Ansprechpartner wurde deutlich, dass gemeinsam genutzte Werkzeuge nicht jederzeit schnell wiedergefunden werden können, da keine zentrale und verlässlich gepflegte Übersicht über Standort, Ausleihstatus und Zustand der Werkzeuge besteht. Vor diesem Hintergrund wurde das vorliegende Projekt als geeigneter Lösungsansatz vorgeschlagen.

Zur Zielgruppe der Anwendung gehören registrierte Mitarbeitende des Labors, die gemeinsam genutzte Werkzeuge im täglichen Arbeitsablauf entnehmen, zurückgeben und verwalten.

## 1.2 Projektziel

Ziel des Projekts ist die Entwicklung einer funktionsfähigen internen Webanwendung, mit der gemeinsam genutzte Laborwerkzeuge strukturiert verwaltet und nachvollziehbar ausgeliehen werden können.

Die Anwendung soll registrierten Benutzerinnen und Benutzern insbesondere ermöglichen,

- Werkzeuge anzulegen und zu verwalten,
- den aktuellen Standort und den Standardablageort zu dokumentieren,
- Werkzeuge aus- und zurückzubuchen,
- den Status eines Werkzeugs, zum Beispiel verfügbar, ausgeliehen oder außer Betrieb, einzusehen und zu ändern,
- relevante Änderungen wie Ausleihe, Rückgabe, Standortwechsel oder Statusänderungen nachvollziehbar zu protokollieren,
- einfache interne Benachrichtigungen bei relevanten Änderungen zu erhalten,
- Such- und Filtermöglichkeiten für Werkzeuge und Statusinformationen zu nutzen.

Durch die Lösung sollen die bisher unzuverlässige manuelle Dokumentation ersetzt, Suchzeiten reduziert und die Nachverfolgbarkeit gemeinsam genutzter Werkzeuge verbessert werden. Außerdem soll die Transparenz im Umgang mit Laborwerkzeugen erhöht und die Effizienz im Laboralltag verbessert werden.

## 1.3 Projektbegründung

Die Durchführung des Projekts ist fachlich begründet, da der bisherige organisatorische Prozess zur Dokumentation von Entnahmen und Rückgaben überwiegend papierbasiert ist und in der Praxis nicht konsistent eingehalten wird. Die bisherige Nachverfolgung erfolgt über ein physisches Formular bzw. Dokument, in dem eingetragen werden soll, wer ein Werkzeug ausgeliehen oder entnommen hat. Dieses Formular wird jedoch nur selten vollständig oder zuverlässig ausgefüllt.

Dadurch ist häufig nicht eindeutig nachvollziehbar, welches Werkzeug sich aktuell wo befindet, wer es zuletzt verwendet hat oder ob es sich noch im Umlauf befindet. Auch der Standardablageort und der aktuelle Zustand eines Werkzeugs sind nicht zentral und durchgängig dokumentiert. Dies führt zu Suchaufwänden, Unterbrechungen im Arbeitsablauf und organisatorischen Unsicherheiten im Team.

Die Entwicklung einer internen Webanwendung stellt daher einen sinnvollen Lösungsansatz dar, um den bisherigen manuellen Prozess durch eine strukturierte digitale Lösung zu ersetzen und die Transparenz, Nachverfolgbarkeit und Effizienz im Laboralltag zu verbessern.

## 1.4 Projektschnittstellen

Die Anwendung wird als interne Webanwendung umgesetzt und richtet sich an registrierte Mitarbeitende des Labors. Fachliche Schnittstellen bestehen insbesondere zum Laborbereich als Auftraggeber bzw. Zielgruppe der Anwendung. Darüber hinaus ist eine Abstimmung mit dem fachlichen Ansprechpartner hinsichtlich Anforderungen, Kernprozessen und gewünschter Funktionen erforderlich. Diese Abstimmung betrifft insbesondere die Verwaltung von Werkzeugen, die Abbildung von Ausleihe und Rückgabe sowie die Definition von Status- und Standortinformationen.

Technische Schnittstellen bestehen innerhalb der Anwendung zwischen Benutzeroberfläche, Backend-Logik und Datenhaltung. Für die Umsetzung werden Python und FastAPI für die Backend-Logik sowie HTML, CSS und JavaScript für die Benutzeroberfläche verwendet. Die Datenhaltung erfolgt über MySQL, der Datenzugriff über SQLAlchemy. Zur Versionskontrolle und Dokumentation des Entwicklungsfortschritts wird GitHub verwendet. Die Entwicklung und die Tests erfolgen lokal.

## 1.5 Projektabgrenzung

Das Projekt ist bewusst auf einen klar abgegrenzten Funktionsumfang beschränkt. Bestandteil des Projekts ist die Konzeption und prototypische Entwicklung einer internen Webanwendung zur Verwaltung, Ausleihe und Nachverfolgung von Laborwerkzeugen.

Nicht Bestandteil des Projekts sind weiterführende Erweiterungen, die über den definierten Kernumfang hinausgehen. Dazu gehört insbesondere eine zukünftige Lösung, bei der Werkzeuge ausschließlich digital über die Anwendung entnommen werden können oder Lager- bzw. Regalplätze zusätzlich digital überwacht oder verwaltet werden. Diese Erweiterungen werden zwar als mögliche spätere Ausbaustufe betrachtet, sind jedoch nicht Teil des vorliegenden Projekts.

Ebenfalls nicht Bestandteil des Projekts ist die Entwicklung einer vollständigen unternehmensweiten Plattform für weitergehende Inventar- oder Lagerverwaltungsprozesse. Der Fokus liegt ausschließlich auf dem beschriebenen Laboranwendungsfall und den hierfür relevanten Kernfunktionen.