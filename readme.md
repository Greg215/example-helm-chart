# Information
1. This is a simple Helm chart template, the template under the friday folder.
2. It can create deployment, ingress, service also support hpa.
3. This example chart will install httpd. 
4. To deploy it, make sure to update the values for other applications.

# Usage
1. Make sure you have a kubernetes cluster ready before the release.
2. helm install --name <The release chart name> ./friday/
3. Also, can use below repo to create a AWS EKS cluster. (https://github.com/Greg215/terraform-aws-eks)

## verify the release
1. kubectl get pods
2. kubectl get services
3. kubectl get deployment
4. Copy the public DNS name of the cluster.
5. In a new browser tab, paste in the public IP address. Add a colon (:) after it. Copy the port number of <The release chart name> from your terminal output (the number after 80: and before the /TCP), and paste it after the colon in the address bar of your browser tab.