### Screen Design
Screen No | Design
------------ | -------------
01 | [Login]


### API End Point

#### API 01: Login



Request Type | API End Point
------------ | -------------
POST | http://localhost/agro/api/user/mobno

:Header:
```javascript
{
    "Content-Type": "application/json"
}
```

:Request:
```javascript
{
    "usrname": "vignesh",
     "usrpassword": "123"
}
```

:Response:
```javascript
{
    "status": 1,
    "message": "Ok"
}
```
### Sub Task (Primary)
- [ ] If Mobile Number exist in Database and [Status=2 or Status=3]
* - [ ] Return response status as 1. We can Navigate the screen to get password.
- [ ] If Mobile Number exist in Database and [Status=1]
* - [ ] Return response status will be 2. We can Navigate the screen to get OTP. 
* - [ ] Also API will send Generated OTP to respective mobile number. 
- [ ] If Mobile Number does not exist in Database we will throw 401 error 



------
