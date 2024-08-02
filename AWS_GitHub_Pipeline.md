## Tolls
- Cloud Provider: AWS
- VCS: GitHub

## Steps
1) ### Create GitHub Repo (with some crud app)
2) ### Create ECR (Elastic Container Registry) for string all your artifact
![img_7.png](img_7.png)
3) ### Developer Tolls -> create CodeBuild to connect your github repository to aws (via OAuth or access token)
![img_6.png](img_6.png)
4) ### add to your code `buildspec.yml` file, something like [buildspec.yml](example%2Fbuildspec.yml) 
![img_5.png](img_5.png)
5) ### add IAM permission policy for ECR
![img_3.png](img_3.png)
![img_4.png](img_4.png)
6) ### Create ECS (Elastic Container Service) Cluster
![img_2.png](img_2.png)
7) ### Create Task Definition for your ECS
![img_1.png](img_1.png)
8) ### go back to cluster -> create Service, but when you rich the loadBalancer chapter execute 9 and 10 steps, ones you will be done with it chose the one you have created LB
![img.png](img.png)
9) ### Create target group 
![img_8.png](img_8.png)
10) ### Create Load Balancer
![img_9.png](img_9.png)
11) ### Add new Security Rule in EC2 instance, go to EC2 -> Security Group -> default
![img_10.png](img_10.png)

