# Task A3
## Submission Information

| Option | Description |
| ------ | ----------- |
| Name   | Lau Jun Hao Benjamin |
| Matriculation Number | A01840840B |
| Link to GitHub Repository | https://github.com/capeguy/cs3219-otot/OTOT_Task_A3/ |
| Instructions | [Below](#foo) |
| Other Relevant Learnings | null |

## Kubectl Commands
### Create Ingress

    kubectl apply -f nginx-ingress.yml
    
### Configure Service

    kubectl apply -f nginx-service.yml
    
### Access Deployed Image Through Service

    kubectl port-forward service/my-nginx 8002:80
    
Navigate to http://localhost:8002 on a Web Browser