# Dream Green Manager v0.5

- Ștergere cu confirmare pentru clienți și lucrări; lucrările se șterg împreună cu înregistrările asociate, clienții numai după eliminarea lucrărilor.
- Restanțe: lucrare finalizată și neîncasată integral SAU scadență depășită.
- Indicator financiar verde / roșu / portocaliu pe Dashboard și lista lucrărilor.
- Culori discrete pentru secțiunile cheltuieli, încasări, activități, suplimentări.
- Rapoarte: zile calendaristice distincte și zile cumulate pe lucrări.
- Baza IndexedDB și celelalte funcții din v0.4 se păstrează.

Înainte de actualizare, exportă backup JSON. Încarcă toate cele 8 fișiere în rădăcina aceluiași repository GitHub Pages, fără a dezinstala aplicația. Testează pe iPhone înainte de utilizare în producție. Notificările push iOS nu sunt implementate.

## Dark Mode
Selector în antet: Automat (urmează tema iPhone), Luminos, Dark (negru cu carduri conturate discret). Preferința este păstrată local pe dispozitiv.


## v0.6 – suplimentări și contacte
- Indicator galben „Lucrări suplimentare” în detaliul lucrării: doar suplimentările aprobate, deja incluse în valoarea totală (nu se dublează).
- Import local de fișier vCard (.vcf) în formularul Clienți, cu nume, telefon, e-mail, adresă și observații. Utilizatorul verifică și salvează manual; nu există acces direct la agenda iOS.
- Pictograme cu fundal negru pentru ecranul principal și favicon. iOS poate păstra pictograma veche în cache.
- Baza de date IndexedDB rămâne neschimbată.
