# Todo and Hello World Rest APIs Connecting to MySQL

- Image URL - https://hub.docker.com/r/in28min/todo-rest-api-mysql
- Image - in28min/todo-rest-api-mysql:1.0.0.RELEASE
- Runs on port 5000
- Run com.in28minutes.rest.webservices.restfulwebservices.RestfulWebServicesApplication as a Java Application.


## Containerization


## Todo JPA Resource URLs

- GET - http://localhost:5000/jpa/users/in28minutes/todos

```
[
  {
    "id": 10001,
    "username": "in28minutes",
    "description": "Learn JPA",
    "targetDate": "2019-06-27T06:30:30.696+0000",
    "done": false
  },
  {
    "id": 10002,
    "username": "in28minutes",
    "description": "Learn Data JPA",
    "targetDate": "2019-06-27T06:30:30.700+0000",
    "done": false
  },
  {
    "id": 10003,
    "username": "in28minutes",
    "description": "Learn Microservices",
    "targetDate": "2019-06-27T06:30:30.701+0000",
    "done": false
  }
]
```


