# Kubernetes-mongo-project
Here I written all the deployment.yml , service.yml,congfig_map,secrets.yml . For the monogo-express application which can be deployed by kubernestes.


step 1 : first deploy the mongo-secret.yaml file . use this command
           kubectl apply -f mongo-secret.yaml
      
step 2 : second deploy the mongo databse use this file mongo-deploy.yaml. use this command 
           kubectl apply -f mongo-deploy.yaml
        
step 3 : third now deploy the configMap for mongo-express applicaton by this file mongo-config.yml file . use this command
                kubectl apply -f mongo-config.yml
now last step ,

step 4 : deploy mongo-express app use this file mongoexpress-deploy.yml. use this command
                kubectl apply -f mongoexpress-deploy.yml
                
         
         now for the check if your application is working fine use this command if you using minikube :
         
         minikube service mongo-express-service   # with command you will go to the browser                                                     and you can see your application is                                                         working fine.
