# Information services

## Microservice try out with fast api
## Information serives uses the auth service function as wrapper and requests (POST call) to check the authorization is correct or not

## Run: uvicorn main:app --reload --port 8081

### example try out

```
>> curl http://127.0.0.1:8000/info/ -i
HTTP/1.1 401 Unauthorized

>> curl http://127.0.0.1:8000/info/ -i --header "Authorization: kishore"
HTTP/1.1 200 OK
{"info":"The information is correct and valid!"}
```
