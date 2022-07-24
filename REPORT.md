# Report / screenshots

## 1. Web Application

- CRUD
We can now [create, read, upadate and delete](/userapi/src/controllers) in controllers
and [create, read, upadate and delete](/userapi/src/routes) in routes too
look tests bellow.

![App Lauching](/img/app-launch.png)



- Tests (npm test)

![App Tests](/img/app-test.png)

## 2. CI/CD

- [Github action], deploy on heroku and dockerhub
![Github Action](/img/ci-cd-github-action.png)

- [Deployment on heroku]()
![Heroku Deployment](/img/heroku.png)

## 3. Vagrant result:

![Vagrant Ansible](/img/vagrantAnsible.png)
- We can see that every thing runs and is well installed with healthcheck result provide at the bottom of the screen shot

![Vagrant result run in browser](/img/vagrantConnectionRedis.png)

- We can see that it is well connected to redis and that there is no user serg in the database

## 4. Docker Image

- Create a docker Image

![Docker Image](/img/docker-image.png)



## 5. Docker Compose

- Lauch Docker Compose sudu docker-compose up

![Lauch docker-compose](/img/compose-launch.png)

- Connect to the app with docker-compos

![connect in browser](/img/compose-connect.png)

## 6. Kubernetes

### Volumes well linked
- Persitent Volume 

![Persitent Volume attached to Persistent Volume Claim](/img/k8s-pv.png)
- Persitent Volume Claim 

![Persitent Volume attached to Persistent Volume Claim](/img/k8s-pvc.png)

- Redis volume 

![](/img/k8s-redis-volume.png)

### Config Map for app deployment environnement varaibles

![config map](/img/k8s-config-maps.png)


### Pods

![Pods](/img/k8s-pods.png)
### Services

![Services](/img/k8s-services.png)
### Well running application
-  Run cluster

![Lauchn app services on  http://192.168.59.101:30000](/img/k8s-connection-cluster.png)
- Connect to cluster on local browser

![Connection on http://192.168.59.101:30000](/img/k8s-connection-success-cluster.png)


## 7. Istio result:

![KialiOverview](/img/kialiOverw.png)
- here we can see the two namespace of the project. The namespace of our application and its microservices named default and the namespace of the istio-system services.

![KialiApp](/img/App.png)
- here we have the two applications of our project named project-devops & redis-deployment. We can also see the health of the applications.

![KialiGraph](/img/graph.png)
- Here we have the routing graph of our applications with kiali. We can see the routing with the two virtual services and the request shiffting. The firsts link between unknown and v1/v2 is http connexion and between v1/v2 and redis deployment is TCP connexion.

- Here we have some informations from kiali tool in the workloads, services and istio-config of our application and there health status:

![KialiWorkload](/img/Wkld.png)
![kialiSvc](/img/Svc.png)
![kialiIstioConf](/img/istioConfig.png)

## 8. Monitoring result:

### Prometheus

- Here we have some informations displaid by prometheus on our application.

![Run&Build](/img/Run&BuildInfo.png)

Status :

![Status](/img/Status.png)

Targets :

![Targets](/img/TargetsProm.png)

Services discovery :

![Services discovery](/img/SvcDiscovery.png)

### Grafana :

Control panel :

![istioControlPanel](/img/istioControlPanel.png)

Performance panel :

![istioPerformance](/img/istioPerformance.png)

Alert :

- here we see how to create an alert and trigger it with grafana by sending an e-mail

![Alertpannel](/img/Alertpannel.png)

![TestRuleAlert](/img/TestRuleAlert.png)

![AlertNotCre](/img/AlertNotCre.png)

![ChannelCreation](/img/ChannelCreation.png)
