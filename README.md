Projekt-Seminar für WInf
website Mängelmelder Nürnberg
Backend mit relationaler Datenbank
kommuniziert mit städtischen Stellen: Einträge werden (je nach Stadt) direkt an kommunale Ämter oder Dienstleister weitergeleitet.
Flutter hat alle nötigen schnittstellen für anforderungen. 

image_picker, camera – Fotos

geolocator, google_maps_flutter – Standort

firebase_messaging – Push Notifications

flutter_local_notifications – Lokale Erinnerungen

http oder dio – API-Zugriffe

shared_preferences – Lokale Benutzerdaten

Mögliches Datenschema: 
id	UUID	Eindeutige ID
titel	String	Kurze Beschreibung
beschreibung	Text	Detaillierte Beschreibung
kategorie	Enum/String	z. B. „Beleuchtung“, „Müll“
bild_url	String	Link zu Bild in Cloud Storage
lat/lng	Float	GPS-Koordinaten
status	Enum	„gemeldet“, „in Bearbeitung“…
user_id	UUID	Wer hat es gemeldet
punkte_vergeben	Boolean	Hat der Melder Punkte erhalten?

Bei Baustellen braucht man interaktion mit einer stadt angestellten oder die teilen ihre datenbank.
