# AWS EKS eksctl Commands
Some popular commands when getting started with [AWS EKS](https://aws.amazon.com/pm/eks/?trk=33d990c1-2a38-472b-9da4-6568a75e9eae&sc_channel=ps&ef_id=Cj0KCQjwuKnGBhD5ARIsAD19RsZ4OEvWatEv87y39O2wT5_4aROQW-Ca4otszInGp-Z2F02GH_OD8p0aAg7AEALw_wcB:G:s&s_kwcid=AL!4422!3!651751059741!e!!g!!aws%20eks!19852662191!145019194777&gad_campaignid=19852662191&gbraid=0AAAAADjHtp_QqWqVkCMk5EpGC6BK5pKiq&gclid=Cj0KCQjwuKnGBhD5ARIsAD19RsZ4OEvWatEv87y39O2wT5_4aROQW-Ca4otszInGp-Z2F02GH_OD8p0aAg7AEALw_wcB) utilizing eksctl.


## Commands
```

# List clusters in a region
eksctl get cluster --region us-east-1


# Get information on nodes in cluster
kubectl get nodes -o custom-columns=NAME:.metadata.name,INSTANCE:.metadata.labels."beta\.kubernetes\.io/instance-type",ZONE:.metadata.labels."topology\.kubernetes\.io/zone"


```