# Gemini API (Spring Boot)

Simple REST API to interact with Gemini AI.

## Base URL

http://localhost:8080/gemini/api

## Endpoint

POST /ask
Send a prompt and get AI response.

## Request

URL
http://localhost:8080/gemini/api/ask

Method
POST

Headers
Content-Type: application/json

Body
{
"prompt": "Hii"
}

## Response

Example
{
"response": "Hello! How can I help you today?"
}

## How to Run

1. Add your API key in application.properties:
   google.api.key=your_api_key_here

2. Run the Spring Boot application

3. Test using Postman or curl

## curl Example

curl -X POST http://localhost:8080/gemini/api/ask 
-H "Content-Type: application/json" 
-d '{"prompt":"Hii"}'

## Notes

* Server runs on port 8080
* Endpoint expects JSON input
* Make sure API key is configured properly
