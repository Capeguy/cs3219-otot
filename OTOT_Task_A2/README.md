# Task A2
## Submission Information

| Option | Description |
| ------ | ----------- |
| Name   | Lau Jun Hao Benjamin |
| Matriculation Number | A01840840B |
| Link to GitHub Repository | https://github.com/Capeguy/cs3219-otot/tree/master/OTOT_Task_A2 |
| Instructions | [Below](#foo) |
| Other Relevant Learnings | null |

## Kubectl Commands
### Deploy Image

    kubectl apply -f nginx-deployment.yml
    
![Create Deployment](images/a2.1.png)

### Configure Service

    kubectl apply -f nginx-service.yml
    
![Create Service](images/a2.2.png)
    
### Access Deployed Image Through Service

Port Forward to service

    kubectl port-forward service/nginx-service 8002:80
    
![Port Forward to Service](images/a2.3.png)
    
Navigate to http://localhost:8002 on a Web Browser

![Access via Web Browser](images/a2.4.png)