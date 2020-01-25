# supermario
supermario on kubernets
there are two ways to run supermario on kubernets 
1) through deployment file
2) using command line 
1) how to create deployment file :- 
    i) create deployment file for example. mario.yaml\
    ii) Now type command : kubectl create -f mario.yaml
    ii) Now check deployment is created or not using kubectl get deployments
    iii) Now run following command : kubectl expose deployment mario-deployment --name=mario --type=NodePort --port=8080 --target-port=8080
    iv) Now check service : kubectl get service 
    v) using service ip run it into browser for example : (ip is 8080:32374 then in browser localhost:32374 OR ip_of_system:32374) 
2)Using Command Line : 
    i) kubectl run mario --image=kaminskypavel/mario
    ii)kubectl get deployment
    iii)  Now run following command : kubectl expose deployment mario-deployment --name=mario --type=NodePort --port=8080 --target-       port=8080
    iv) Now check service : kubectl get service 
    v) using service ip run it into browser for example : (ip is 8080:32374 then in browser localhost:32374 OR ip_of_system:32374) 




:) Tell Me if it Runs
