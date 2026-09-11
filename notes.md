### API 
---
```Application programming interface that enables communication bw different applications```


### Webfundamentals
---

## client server architeture
    ```client sends an http request to server, server process the http request and send back http response ```

### http_methods
---
`GET` => fetch all resources  
`POST` => create an new resource  
`PUT` => update a resource  
`PATCH` => UPDATE a resource (partial update)  
`DELETE` => delete a resource  


### http_request_format
---

`url`  
`http_method`  
`Authorization`  
`body`  

### sample api end point
---

```
Employee

id  name    age   department  salary

1   haris    23          hr      25000
2   vipin    23          qa      25000
3   jithn    23          it      25000
4   rahul    23          hr      25000

```

```
http_request for adding employee

url: localhost:8000/employee/
method:POST
body:{
    "name":"vysak",
    "age":24,
    "department":"hr",
    "salary":45000
}



```
---
```
http_request for listing employee

url:localhost:8000/employee/
method:GET

```

---
```
http_request for fetching specific employee detail

url : localhost:8000/employee/4/
method:GET

```

```
http_request for updating an employee 

url:localhost:8000/employee/4/
method:PUT
body:{
    "name":"Rahul",
    "age":24,
    "department":"hr",
    "salary":30000
}

```

```
http_request for deleting  specific employee 

url:localhost:8000/employee/4/
method:DELETE
```

### Movie task

```
Movie

id      title      year     language        run_time


1          kgf1      2008      kannada           160
2          kgf2      2020      kannada           165
3          kgf3      2026      kannada           167
4          kgf4      2028      kannada           168
5          kgf5      2030      kannada           169
```

`http_request for adding new movie`

url: localhost:8000/movies/  
method: post

body   : {  
    "title": "kgf6",  
    "year": 2032,  
    "language": "kannada",  
    "run_time": 170  
}

`http_request for list all movie`

url : localhost:8000/movies/  
method : get    

`http_request for fetching movie detail`

url : localhost:8000/movies/5/  
method : get  

`http_request for update movie`

url : localhost:8000/movies/5/  
method : put  
body {  
    "title":"kgf5",  
    "year":2030,  
    "language":"Kannada"  
    "run_time:175  
}
`http_request for delete movie`

url : localhost:8000/movies/5/  
method : delete  


## Hospital task
Hospital  

id    name              place       phone          specialization  

1     amrita hospital   kochi       9876543210     cardiology  
2     aster hospital    kochi       9876543211     neurology  
3     jubilee hospital  thrissur    9876543212     dentist  
4     medical trust     kochi       9876543213     pediatrics  
5     appolo hospital   tvm         9876543214     physician  

`http_request for adding new hospital`  
url: localhost:8000/hospitals/  

method: post  

body: {  
    "name": "amrita hospital",  
    "place": "kochi",  
    "phone": "9876543210",  
    "specialization": "cardiology"  
}

`http_request for list all hospital`  

url: localhost:8000/hospitals/  

method: get  
 
`http_request for fetching hospital detail`  

url: localhost:8000/hospitals/5/  

method: get   

`http_request for update hospital`  

url: localhost:8000/hospitals/5/  

method: put  

body: {  
    "name": "appolo hospital",  
    "place": "kollam",   
    "phone": "9876543299",  
    "specialization": "cardiology"  
}

`http_request for delete hospital`  

url: localhost:8000/hospitals/5/  

method: delete  