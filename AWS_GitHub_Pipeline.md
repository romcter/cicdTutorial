## Tolls
- Cloud Provider: AWS
- VCS: GitHub

## Steps
1) ### Create GitHub Repo (with some crud app)
2) ### Create ECR (Elastic Container Registry) for string all your artifact
![img_7.png](screenshots/img_7.png)
3) ### Developer Tolls -> create CodeBuild to connect your github repository to aws (via OAuth or access token)
![img_6.png](screenshots/img_6.png)
4) ### add to your code `buildspec.yml` file, something like [buildspec.yml](example%2Fbuildspec.yml) 
![img_5.png](screenshots/img_5.png)
5) ### add IAM permission policy for ECR
![img_3.png](screenshots/img_3.png)
![img_4.png](screenshots/img_4.png)
6) ### Create ECS (Elastic Container Service) Cluster
![img_2.png](screenshots/img_2.png)
7) ### Create Task Definition for your ECS
![img_1.png](screenshots/img_1.png)
8) ### go back to cluster -> create Service, but when you rich the loadBalancer chapter execute 9 and 10 steps, ones you will be done with it chose the one you have created LB
![img.png](screenshots/img.png)
9) ### Create target group 
![img_8.png](screenshots/img_8.png)
10) ### Create Load Balancer
![img_9.png](screenshots/img_9.png)
11) ### Add new Security Rule in EC2 instance, go to EC2 -> Security Group -> default
![img_10.png](screenshots/img_10.png)

