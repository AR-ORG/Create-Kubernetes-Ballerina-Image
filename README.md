# Create-Kubernetes-Ballerina-Image

# Kubernetes images using Ballerina 

  1.  Clone this git repository 
  
  2.  Edit the *.bal files with details of your image, ServicePort, Payload Text
  
  3.  docker login --- Add your credentials 
  
  4.  ballerina build ballerina_app_v1.bal
  
  5.  docker images -- Get your image
  
  6.  docker push harshal0812/ballerinav1
  
  7. Deploy your app as - 
  
      1.  kubectl apply -f /root/ballerina_files/kubernetes/
      
                                  OR
                                  
      2.  helm install --name ballerinav1deployment /root/ballerina_files/kubernetes/ballerinav1deployment
