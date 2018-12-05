pipeline {
    agent {
        label 'eabuild-1'
    }
    
    stages {
         stage ("check out") {
             steps {
                 checkout scm
             }
         }
         stage ("docker build") {
             steps {
                 bat "docker build -t hello-node ."
             }
         }
    }
}