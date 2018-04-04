# mountebank-service
run ./start_mb.sh

GET: http://localhost:4545/test/success
response:
{
    "status": "success",
    "message": "",
    "data": []
}

GET: http://localhost:4545/test/fail
response:
{
    "status": "error",
    "message": "",
    "data": []
}