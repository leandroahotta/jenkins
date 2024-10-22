// pipeline {  
//     environment {
//       registry = "osanamgcj/mobead_image_build"
//       registryCredential = 'dockerhub'
//       dockerImage = ''
//     }
//     agent any 
//     stages { 
//         stage('Lint Dockerfile'){ 
//             steps{
//                 echo "Pipeline Usando Jenkinsfile"
//                 sh 'docker run --rm -i hadolint/hadolint < Dockerfile'
//             }
//         }
//         stage('Build image') {
//             steps{
//                 script {
//                     dockerImage = docker.build registry + ":$BUILD_NUMBER"
//                 }
//             }
//         }
//         stage('Delivery image') {
//             steps{
//                 script {
//                   docker.withRegistry('https://registry-1.docker.io/v2/', 'dockerhub') {
//                    dockerImage.push("$BUILD_NUMBER")
//                   }
//                 }
//             }
//         }
//     } 
// }
pipeline {
    agent any
    stages {
        stage('Step1') {         
            steps {
                echo 'step 1'
                sh 'printenv'
            }
        }
        stage('Step2') {
            steps {
                echo 'step 2'
            }
        }
        stage('Step3') {   
            steps {
                echo 'step 3'
            }
        }
    }
}