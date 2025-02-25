pipeline {
    agent any

    stages {
        stage('terraform init') {
            steps {
                withCredentials([azureServicePrincipal('welcome')]) {
                    sh '''
                    cd /home/welcomeuser/practice/RG
                    terraform init
                    terraform plan
                    terraform apply -auto-approve
                    '''
                }
            }
        }
    }
}


// pipeline {
//     agent any
//     stages {
//         stage('isntall nginx') {
//             steps {
//                 sh '''sudo apt-get update
//                 sudo apt-get install -y nginx
//                 sudo nginx -v'''
//             }
//         }
//     }
// }
