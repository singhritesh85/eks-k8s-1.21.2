```
For Any New kubernetes version just update eksctl version and kubernetes version in the script
```









# eks-k8s-1.21.2

A nodegroup can be scaled by using the eksctl scale nodegroup command:

eksctl scale nodegroup --cluster=<clusterName> --nodes=<desiredCount> --name=<nodegroupName> [ --nodes-min=<minSize> ] [ --nodes-max=<maxSize> ]
  
example:-  eksctl scale nodegroup --name=test-nodegroup2 --cluster=test --nodes=2 --region=us-east-2
  
                     or 
  
           eksctl scale nodegroup --name=test-nodegroup2 --cluster=test --nodes=4 --region=us-east-2 --nodes-min=2 --nodes-max=5
