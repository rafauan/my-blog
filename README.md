
# Blog Strapi - API

## Funkcjonalność

Prosty projekt postawiony na Strapi i SQLite, który pozwala na dodawanie nowych postów blogowych.

## Uruchomienie projektu
### `Instalacja`
```
npm install
# or
yarn install
```

### `develop`
```
npm run develop
# or
yarn develop
```
### `start`
```
npm run start
# or
yarn start
```
### `build`
```
npm run build
# or
yarn build
```


## Lista endpointów

Endpointy testujemy przy pomocy adresu **http://localhost:1337/api/**

W panelu administratora został wygenerowany API Token umożliwiający działa na niepublicznych endpointach.
 
Kolekcja **Posts** 
 - /posts (GET) - listowanie wszystkich postów w bazie
 - /posts (POST) - dodanie nowego postu (wymaga autoryzacji poprzez Bearer Token)
 - /posts/{post} (GET) - otrzymanie informacji tylko o jednym poście
 - /posts/{post} (PUT) - zmiana informacji dla jednego postu (wymaga autoryzacji poprzez Bearer Token)
 - /posts/{post} (DELETE) - usunięcie wybranego postu (wymaga autoryzacji poprzez Bearer Token)
  
Kolekcja **Categories** 
 - /categories (GET) - listowanie wszystkich kategorii w bazie
 - /categories (POST) - dodanie nowej kategorii (wymaga autoryzacji poprzez Bearer Token)
 - /categories/{category} (GET) - otrzymanie informacji tylko o jednej kategorii
 - /categories/{category} (PUT) - zmiana informacji dla jednej kategorii (wymaga autoryzacji poprzez Bearer Token)
 - /categories/{category} (DELETE) - usunięcie wybranej kategorii (wymaga autoryzacji poprzez Bearer Token)

Więcej informacji jest zawarta w pliku **api_doc.json**. Można zaimportować go np. do programu Postman.