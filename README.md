# The Blog Service

## Register Blogger

`POST /blogger`
```json
{
  "email": "hdoe@apper.ph",
  "name": "John Doe",
  "password": "jdoe123"
}
```
1. All fields are required.
2. Email format must be valid.
3. Password must be at least 5 characters.

`Response: 201 - Created`
```json
{
  "id": "<UUID>",
  "date_registration": "2023-07-11T23:23:12"
}
```

## Get Blogger

`GET /blogger/{id}`

`Response: 200 - OK`
```json
{
  "id": "<UUID>",
  "name": "John Doe",
  "email": "jdoe@apper.ph",
  "date_registration": "2023-07-11T23:23:12"
}