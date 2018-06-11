pipeline {
   agent any
   tools {
    go 'Go 1.10.3'
    }  
   stages {
       stage('Preparation') {
           steps {
            sh "go get -v -d"
           }
       }
       stage('Test') {
           steps {
            sh "go test -v -cover"
           } 
       }
       stage('Results') {
           steps {
            sh "rm -rf *"
            echo "Results"
           }
       }
   } 
}
