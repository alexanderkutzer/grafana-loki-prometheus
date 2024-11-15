# grafana-loki-prometheus
## Einführung in Logging und Monitoring

### 1. Warum Monitoring und Logging wichtig sind
- Warum ist es wichtig, Logs und Metriken in modernen Anwendungen zu überwachen?
-> es ist wichtig, um die Performence, Stabilität und die Sicherheit von Systemen zu überwachen und zu gewährleisten. 

- Was könnten wir aus Logs und Metriken über das Verhalten eines Systems lernen?
-> Logs helfen uns Fehler zu identifizieren
-> Metriken hingegen geben und Einblicke in die Systemressourcen un die Performence

### 2. Grafana, Loki und Promtail
- Was wäre der Vorteil, Logs zentral zu speichern und zu visualisieren, anstatt sie nur lokal zu durchsuchen?
-> durch eine zentrale Speicherung von Logs vereinfacht die Verwaltung, Suche und Analyse von Logs aus unterschiedlichen Quellen. So können z.B. Muster, Probleme schneller erkannt werden ohne jedes System einzeln durchsuchen zu müssen

- Wie könnten Tools wie Grafana und Loki bei der Fehlerbehebung helfen?
-> Loki ist für die Speicherung von Logs zuständig
-> Grafana für die übersichtliche Visualisierung der Daten. 
Mithilfe gezielter Abfragen kann man Fehler schnell lokalisieren und analysieren.

### 3. Übergang zu Prometheus
- Logs sagen uns, *was* passiert ist – wie könnten Metriken uns dabei helfen, *wie oft* oder *wie lange* etwas passiert ist, zu verstehen?
-> Logs geben uns Details zu einzelnen Vorfällen (z.B. Timeout-Fehler)
-> Metriken zeigen quantitative Daten wie die Häufigkeit und Dauer von Ereignissen (z.B. wie oft der Timeout-Fehler augetreten ist, ... )


- Was könnten Beispiele für wichtige Metriken in einer Anwendung sein? (z. B. Antwortzeiten, Anzahl der Anfragen)
-> Durchschnittliche, maximale und minimale Zeit für Anfragen. Gesamte Anfragen pro Sekunde oder Minute.Anteil der fehlgeschlagenen Anfragen (z. B. HTTP 4xx) Nutzung der Systemressourcen (CPU Auslastung)

### 4. Verknüpfung der Tools
- Wie könnten Loki, Promtail, Grafana und Prometheus zusammenarbeiten, um ein vollständiges Monitoring- und Logging-System aufzubauen?
->
- Prometheus überwacht Metriken, Loki speichert die Logs
- mit Grafana werden beide Datenquellen kombiniert und visualisiert
