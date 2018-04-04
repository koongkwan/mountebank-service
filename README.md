# mountebank-service
- npm install -g mountebank

- run ./start_mb.sh

`
GET: http://localhost:4545/test/success
response:
"statusCode": 200
{
    "status": "success",
    "message": "",
    "data": []
}
`
GET: http://localhost:4545/test/fail
"statusCode": 200
response:
{
    "status": "error",
    "message": "",
    "data": []
}

GET: http://localhost:4545/test/fail/400
"statusCode": 400
response:
{
    "status": "error",
    "message": "bad request",
    "data": []
}

GET: http://localhost:4545/test/fail/500
"statusCode": 500
response:
{
    "status": "error",
    "message": "internal server error",
    "data": []
}
