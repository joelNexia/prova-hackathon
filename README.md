 ## PROVA HACKTHON BARCELONA ACTIVA

 Aquesta prova esta fet en laravel (php framework).

# ENDPOINTS

### Endpoints Table

### Ruta principal url/appActivitats/.... 

| HTTP Method | Endpoint                     | Description                                             | Request Data (Body/Query)                                                                                           | Response                                             |
|-------------|------------------------------|---------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------|------------------------------------------------------|
| `GET`       | `/usuaris`                    | List all users (usuaris)                                 | N/A                                                                                                                 | JSON array of `usuaris`                              |
| `POST`      | `/usuaris`                    | Create a new `usuari`                                    | `{ "nom": "John", "cognom": "Doe", "edad": 25, "email": "johndoe@example.com", "password": "secret" }`               | Newly created `usuari` (JSON)                        |
| `GET`       | `/usuaris/{id}`               | Get a single `usuari` by ID                              | `id` (URL parameter)                                                                                                | Single `usuari` object (JSON)                        |
| `PUT/PATCH` | `/usuaris/{id}`               | Update an existing `usuari`                              | `{ "nom": "Jane", "cognom": "Doe", "edad": 26, "email": "janedoe@example.com" }`                                     | Updated `usuari` object (JSON)                       |
| `DELETE`    | `/usuaris/{id}`               | Delete a `usuari`                                        | `id` (URL parameter)                                                                                                | Deletion success message (JSON)                      |
| `POST`      | `/activitats`                 | Create a new `activitat`                                 | `{ "name": "Basketball", "description": "Sport Activity", "date": "2024-01-10" }`                                    | Newly created `activitat` (JSON)                     |
| `GET`       | `/activitats`                 | List all activities (activitats)                         | N/A                                                                                                                 | JSON array of `activitats`                           |


