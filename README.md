 ## PROVA HACKTHON BARCELONA ACTIVA

 Aquesta prova esta fet en laravel (php framework).

# ENDPOINTS

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
| `POST`       | `/activitats/apuntar`                 | Apunta un usuari a una activitat                         | `{ "usuari_id": 1, "activitat_id": 1,                                                                                                                |  `message`  (JSON)                         |


