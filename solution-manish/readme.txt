Dockerfile: which create the docker image of the prediction model.
k8s-deployment.yaml : all the configution in order to deploy the solution in k8s cluster 
Note : for production we can user ingress for applying ssl cert not mentioned in this as done on local with naked ip.

chnges:
    app.py : written statement for excution of the code over public ip(0.0.0.0) and port 8000is assigned.
    MAkefile :  contains all the command for doing deployment nad creation of docker image.