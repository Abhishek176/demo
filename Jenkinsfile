pipeline {
    agent any
    tools {
        terraform 'terraform'
    }
    stages {
        stage ("Terraform init and apply") {
            steps {
                sh "terraform init /var/lib/jenkins/workspace/demo"
                sh "terraform apply -auto-approve"
            }
        }
    }
}
