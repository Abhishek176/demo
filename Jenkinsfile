pipeline {
    agent any
    tools {
        terraform 'terraform'
    }
    stages {
        stage ("Terraform init and apply") {
            steps {
                sh "terraform init"
                sh "terraform apply -auto-approve"
            }
        }
    }
}
