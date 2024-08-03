---
openapi: /people/search
---

# People Search

The People Search endpoint allows you to search for individuals based on their first name, last name, city, and state abbreviation.

## Endpoint

**POST** `/people/search`

## Request Body

The request body should be a JSON object containing the following properties:

- `first_name` (string): The first name of the person you are searching for. Example: `John`.
- `last_name` (string): The last name of the person you are searching for. Example: `Doe`.
- `city` (string): The city where the person resides. Example: `New York`.
- `state_abv` (string): The state abbreviation where the person resides. Example: `NY`.

### Example Request

```json
{
  "first_name": "John",
  "last_name": "Doe",
  "city": "New York",
  "state_abv": "NY"
}
