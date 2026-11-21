# Dream Green Manager Offline — prototip PWA 0.2

Refacere offline-first pornind de la arhiva Flask/SQLite `dreamgreen-manager-render-test(1).zip`. Este un prototip nou, nu o actualizare automată a aplicației Render.

## Funcții disponibile
Clienți, lucrări, cheltuieli, încasări, activități, suplimentare, calendar local, dashboard, raport anual/top lucrări/top clienți/profit pe zi; IndexedDB local; export și restaurare JSON.

## Publicare și instalare
1. Publică **conținutul** acestui director pe un hosting static HTTPS (de exemplu GitHub Pages). Nu se poate instala ca PWA offline direct din ZIP sau `file://`.
2. Deschide URL-ul HTTPS în Safari pe iPhone, așteaptă încărcarea completă, apoi Share → Adaugă pe ecranul principal.
3. Deschide aplicația din pictograma instalată, introdu câteva date de test și verifică după închidere și în modul Avion.
4. În Backup, apasă Exportă, apoi salvează fișierul în Fișiere → iCloud Drive. Verifică în Fișiere că există. Testează restaurarea pe un set de date de test.

## Limitări importante
- Backup în iCloud este **manual**, nu automat. Browserul nu poate garanta salvarea directă automată în iCloud Drive.
- IndexedDB poate fi eliminat de iOS sau la ștergerea datelor Safari / a aplicației. Nu folosi pentru date critice fără copii externe verificate.
- Nu există sincronizare Google Calendar/Contacts, editare înregistrări, autentificare sau criptare de backup în această versiune.
- Rapoartele sunt de marjă brută estimată, fără alocarea costurilor fixe sau taxe. Zile lucrate = număr de date distincte cu activități.
- Nu există migrare automată din SQLite; datele din aplicația Render nu sunt importate.
- Nu încărca backup-urile JSON necriptate pe spații publice.
- Pentru utilizare în producție sunt necesare testare pe iOS, gestionarea actualizărilor cache, protecția datelor și eventual export criptat.
