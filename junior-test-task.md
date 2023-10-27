# Junior Test Task

## General Requirements

The project under development should be built using the .NET 7 stack.

The project under development should have a UI in the form of a Swagger client.

The project under development should implement 2 REST requests.

All server requests must be restricted to authenticated users, and BASIC authentication should be used as the authentication method.

Communication between the server and the client should use a text data format - JSON.

As a data source, the implementation should use one of the services on the internet (for example).

The application should be runnable in a Docker container.

## Requirements for the MoskowWeather Request

This request, when provided with a date as a query parameter, should return the temperature in Moscow on the current date (any of the values obtained on that date) as the response.

## Requirements for the SaveMoskowWeather Request

This request, when provided with a date as a query parameter, should save the temperature value in Moscow on the current date (any of the values obtained on that date) in a relational database (use one of the following databases for implementation: Postgres, MySQL, MS SQL, Oracle) and return the saved value as the response.
