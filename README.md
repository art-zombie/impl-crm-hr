# WORKERS
---
###GET
- вывести всех работников
```
http://localhost:8084/hr/workers
```
- вывести работника с id n
```
http://localhost:8084/hr/workers/n
```
- вывести работающего работника c должностью n
```
http://localhost:8084/hr/workers/working/n
```
- получить всех работающих работников должности n
```
http://localhost:8084/hr/workers/working/n
```
###POST
* добавить работника (json)
```
http://localhost:8084/hr/workers
```
```
{  
  "positionId": 1,
  "name": "Andrey",
  "patronymic": "Andreev",
  "email": "Andrey@gmail.com",
  "phone": "12345",
  "salary": 123.4,
  "isWorking": true
}
```
###PUT
- корректировать n-ого работника (json)
```
http://localhost:8084/hr/workers/n
```
``` 
{
  "positionId": x,
  "name": "x",
  "patronymic": "x",
  "email": "x",
  "phone": "x",
  "salary": x,
  "isWorking": x
}
```
###DELETE
- удалить n-ого работника
```
http://localhost:8084/hr/workers/n
```
---
# SHEDULES
---
###GET
- вывести все расписания
```
http://localhost:8084/hr/shedules
```
- вывести n-ое расписание
```
http://localhost:8084/hr/shedules/n
```
###POST
- добавить расписание (json)
```
http://localhost:8084/hr/shedules
```
```
{
    "id" : 1,
    "hoursPerWeek" : 5.5,
    "vacationDays" : 6,
    "vacationSchedule" : 7
}
```
###PUT
- корректировать n-ое расписание (json)
```
http://localhost:8084/hr/shedules/n
```
```
{
    "id" : x,
    "hoursPerWeek" : x,
    "vacationDays" : x,
    "vacationSchedule" : x
}
```
###DELETE
- удалить n-ое расписание
```
http://localhost:8084/hr/shedules/n
```
---
# POSITIONS
---
###GET
- вывести все должности
```
http://localhost:8084/hr/positions
```

- вывести n-ую должность
```
http://localhost:8084/hr/positions/n
```
###POST
- добавить должность (json)
```
http://localhost:8084/hr/positions
```
```
{
    "position" : "Директор"
}
```
###UPDATE
- корректировать n-ую должность (json)
```
http://localhost:8084/hr/positions/n
```
```
{
    "position" : "x"
}
```
###DELETE
- удалить n-ую должность
```
http://localhost:8084/hr/positions/n
```