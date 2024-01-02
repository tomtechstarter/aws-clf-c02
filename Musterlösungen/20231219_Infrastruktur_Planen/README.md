# Mein erstes API

## Allgemeine Infrastruktur
![](./images/Infrastructure.png)

## API Dokumentation
`GET /allitems`: Gibt Alle Elemente der Shopping Liste zurück

`GET /itembyid/{itemId}`: Gibt ein einzelnes Element zurück.
**Parameter**: `itemId` - Einzigartige Id des Elements

`POST /item`: Erstellt ein einzelnes Element.

`DELETE /itembyid/{itemId}`: Löscht ein einzelnes Element.
**Parameter**: `itemId` - Einzigartige Id des Elements

`PUT /itembyid/{itemId}`: Aktualisiert ein einzelnes Element.
**Parameter**: `itemId` - Einzigartige Id des Elements
 
