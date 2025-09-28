### deploy `v2.yml` config:

```
> kubectl create -f v2.yml
service/mywebapp-service created
deployment.apps/mywebapp-deploy created
>
>
> kubectl get all
NAME                                  READY   STATUS    RESTARTS   AGE
pod/mywebapp-deploy-c8666dbd4-5jtdx   1/1     Running   0          20s
pod/mywebapp-deploy-c8666dbd4-7j554   1/1     Running   0          20s

NAME                       TYPE           CLUSTER-IP     EXTERNAL-IP   PORT(S)        AGE
service/kubernetes         ClusterIP      10.96.0.1      <none>        443/TCP        4h59m
service/mywebapp-service   LoadBalancer   10.99.138.35   <pending>     80:30989/TCP   20s

NAME                              READY   UP-TO-DATE   AVAILABLE   AGE
deployment.apps/mywebapp-deploy   2/2     2            2           20s

NAME                                        DESIRED   CURRENT   READY   AGE
replicaset.apps/mywebapp-deploy-c8666dbd4   2         2         2       20s
```


