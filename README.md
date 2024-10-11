 ## PROVA HACKTHON BARCELONA ACTIVA

 Aquesta prova esta fet en laravel (php framework).

 ### Preparació 

 Introduir les ordres en la terminal a l'arrel del projecte.
```bash
composer update
```

Install dependencies
```bash 
composer install
```

Load files and clear any cache
```bash 
composer dump-autoload

Configurar la conexió a la base de dades

crear `.env` a l'arrel del projecte
```php
#Database connection

DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=laravel
DB_USERNAME=root
DB_PASSWORD=
```
Per ultim fer aquesta ordre.
```bash 
php artisan migrate
```

### Endpoints Table

#### Ruta principal `url/appActivitats/....`

| HTTP Method | Endpoint                     | Descrició                                             | Request Data (Body/Query)                                                                                           | Resposta                                             |
|-------------|------------------------------|---------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------|------------------------------------------------------|
| `GET`       | `/users/{id}`                    | Mostra un usuari                                  | N/A                                                                                                                 | JSON array of `usuaris`                              |
| `POST`      | `/user`                    | Crea un nou `usuari`                                    | `{ "nom": "John", "cognom": "Doe", "edad": 25, "email": "johndoe@example.com"}`               | `message` `user` (JSON)                        |
| `PUT`       | `/users/{id}`               | Actulitza `usuari` by ID                              | `id` (URL parameter)                                                                                                | `message` `usuari` (JSON)                        |
| `DELETE` | `/users/{id}`               | Elimina un `usuari`                              | N/A                                     |  `message`  (JSON)                       |
| `POST`    | `/activitat`               | Crea una nova `activitat`                                        | `{ "nom": "Basketball", "descripcio": "Sport Activity", "capacitat_maxima": 10 }`                                                                                               |  `message` `activitat` (JSON)                      |
| `GET`      | `/activitats`                 | Torna totes les `activitat`                                 |                                     |  JSON array de `activitats`                     |
| `POST`       | `/activitats/apuntar`                 | Apunta un usuari a una activitat                         | `{ "usuari_id": 1, "activitat_id": 1}`                                                                                                                |  `message`  (JSON)                         |


