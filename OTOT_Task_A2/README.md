# Task A2
## Submission Information

| Option | Description |
| ------ | ----------- |
| Name   | Lau Jun Hao Benjamin |
| Matriculation Number | A01840840B |
| Link to GitHub Repository | https://github.com/capeguy/cs3219-otot/OTOT_Task_A2/ |
| Instructions | [Below](#foo) |
| Other Relevant Learnings | null |

## Kubectl Commands
### Deploy Image

    kubectl apply -f nginx-deployment.yml
    
![Create Deployment](a2.1.png)

### Configure Service

    kubectl apply -f nginx-service.yml
    
![Create Service](a2.2.png)
    
### Access Deployed Image Through Service

Port Forward to service

    kubectl port-forward service/nginx-service 8002:80
    
![Port Forward to Service](a2.3.png)
    
Navigate to http://localhost:8002 on a Web Browser

![Access via Web Browser](a2.4.png)