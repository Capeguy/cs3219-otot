# Task A1
## Submission Information

| Option | Description |
| ------ | ----------- |
| Name   | Lau Jun Hao Benjamin |
| Matriculation Number | A01840840B |
| Link to GitHub Repository | https://github.com/Capeguy/cs3219-otot/tree/master/OTOT_Task_A1 |
| Instructions | [Below](#foo) |
| Other Relevant Learnings | null |

## Instructions on how to run the Docker container

Write index.html
```
<!DOCTYPE html>
<html>

<head>
    <title>CS3219 Task A1</title>
</head>

<body>
    <h1>Hello! This is the HTML page served from NGINX.</h1>
</body>

</html>
```

Write Dockerfile
```
FROM nginx:stable
COPY ./index.html /usr/share/nginx/html/index.html
EXPOSE 80
```

Build & Run Container
        
    docker build . -t capeguy/task_a:latest

![Running of Docker Build](images/a1.1.png)

    docker push capeguy/task_a:latest 

![Running of Docker Push](images/a1.2.png)

    docker run -p "8001:80" capeguy/task_a:latest

![Running of Docker Run](images/a1.3.png)
    
Replace `capeguy` with your own Dockerhub Username

Navigate to http://localhost:8001 on a Web Browser

![Opening in Web Browser](images/a1.4.png)