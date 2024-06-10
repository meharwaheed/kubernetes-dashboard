Last Modified : June 10.2024
---------------------------------------------------------
# K8s Dashboard with NodePort in 4 simple steps
---------------------------------------------------------
1. Clone  K8s-Dashboard repo to deploy it with automation:
`git clone git@github.com:meharwaheed/kubernetes-dashboard.git`
2. Expose dashboard publicly using ingress
   1. Add domain/subdomain in the ingress.yml
3. Read through the YAML files and apply to your cluster to install & configure dashboard properly:
   `kubectl apply -f ./kubernetes-dashboard/`
4. Open your domain on the browser, it will show you log in page
   1. Run this command to create token to be used at the login page
      `kubectl -n kubernetes-dashboard create token admin-user`

Enjoy your shiny new cluster dashboard ! 
