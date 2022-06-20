pipeline {
     agent any
    stages {
       
         // Uploading Docker images into Docker Hub
   
    stage ('K8S Deploy') {
        steps {
              sh 'az login --identity'
              sh 'az account show'
              sh 'az aks get-credentials -g Hzm_RG -n TestAKS'
              sh 'kubectl version'
              sh 'kubectl run nginx --image=nginx --restart=Never'
                
               
        }
    }
    }
}
