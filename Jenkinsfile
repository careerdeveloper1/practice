pipeline {
    agent any

    stages {
        stage('terraform init step') {
            steps {
                withCredentials([azureServicePrincipal('welcome')]) {
                    sh '''
                    cd /home/welcomeuser/practice/RG
                    terraform init
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
