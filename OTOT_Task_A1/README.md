# Task A1
## Submission Information

| Option | Description |
| ------ | ----------- |
| Name   | Lau Jun Hao Benjamin |
| Matriculation Number | A01840840B |
| Link to GitHub Repository | https://github.com/capeguy/cs3219-otot/OTOT_Task_A1/ |
| Instructions | [Below](#foo) |
| Other Relevant Learnings | null |

## Instructions on how to run the Docker container
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