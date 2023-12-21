# Attestation-Java 2 course.

# Примеры запросов
``` .http
@name=GetTask
GET https://localhost:8080/api/v1/task?Num=Р’Р°С€РќРѕРјРµСЂР’Р°СЂРёР°РЅС‚Р°
Content-Type: application/json

###

@name=GetTestValues
GET https://localhost:8080/api/v1/test?taskId=Р’Р°С€РќРѕРјРµСЂРўР°СЃРєРё
Content-Type: application/json

###

@name=SubmitTask
POST https://localhost:8080/api/v1/submit
Content-Type: application/json

{
    "task_id": 1,
    "output": [{"case_id": {"a": 1}}]
}

###

@name=SubmitTaskResponse
HTTP/1.1 200 OK
Content-Type: application/json

{
   "status": "passed",
   "description": "Р—Р°РґР°РЅРёРµ РІС‹РїРѕР»РЅРµРЅРѕ СѓСЃРїРµС€РЅРѕ"
}
```
