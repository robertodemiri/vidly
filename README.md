# Vidly API-Nextflix Clone

La seguente è una RESTful API scritta completamente in Javascript (Node.js + Express.js) + Mongoose (MongoDB DBMS non relazionale)

Il Server HTTP rimane in ascolto sulla porta 3000 su localhost, invece su applicazioni cloud gira sulla porta assegnatali dall'applicazione stessa
L'applicazione è strutturata nel seguente modo:
  - Config (cartella che contiene file di configurazione)
  - Middleware (file.js che contengono funzioni utili per il refactoring del codice)
  - Model (cartella che contiene la struttura delle collezioni (tabelle) del DB)
  - Routes (cartella che contiene tutti i router)
  index.js (main file)
  
Customers.js
GET api/customers/
GET api/customers/:id READ
POST api/customers/ CREATE
PUT api/customers/:id UPDATE
DELETE api/customers/:id DELETE

Genres.js
GET api/genres/ READ
GET api/genres/:id READ
POST api/genres/ CREATE
PUT api/genres/:id UPDATE
DELETE api/genres/:id DELETE

Movies.js
GET api/movies/ READ
GET api/movies/:id READ
POST api/movies/ CREATE
PUT api/movies/:id UPDATE
DELETE api/movies/:id DELETE

Rentals.js (tabella 'pivot')
GET api/rentals/ READ
GET api/rentals/:id READ
POST api/rentals/ CREATE

Users.js
GET api/users/me READ (per poter accedere a questo percorso bisogna prima autenticarsi)
POST api/users/ UPDATE

Auth.js
POST api/auth LOGINS

Per poter eseguire la RESTful API bisogna installare sulla propria macchina Node.js, MongoDB e POSTMAN (non ho costruito un'applicazione front-end)

