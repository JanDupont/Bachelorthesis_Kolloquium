# Frage

Was passiert, wenn der Browser bei erhalt einer Push-Nachricht vollständig geschlossen ist?

Push-Benachrichtigungen werden an den Service Worker geliefert, auch wenn der Browser vollständig geschlossen ist. Der Service Worker läuft im Hintergrund und kann Push-Nachrichten auch dann empfangen, wenn der Browser nicht geöffnet ist.

Wenn eine Push-Nachricht vom Service Worker empfangen wird, kann er die Nachricht im IndexedDB-Speicher des Browsers zur späteren Verarbeitung speichern. Dadurch kann der Service Worker die empfangenen Push-Nachrichten verfolgen und sie dem Benutzer beim nächsten Öffnen des Browsers anzeigen.

# Frage

Der Service-Worker ist also auch dann aktiv, wenn der Browser vollständig geschlossen ist?

Ja, das ist richtig.  
Der Service Worker ist ein Hintergrundprozess, der von der browserseitigen JavaScript-Engine ausgeführt wird. Er läuft unabhängig von der Benutzeroberfläche des Browsers und kann Nachrichten empfangen, verarbeiten und speichern, auch wenn der Browser vollständig geschlossen ist.
