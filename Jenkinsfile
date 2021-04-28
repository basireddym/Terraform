pipeline{
    agent any
    stages{
        stage('GIT Clone'){
            steps{
                git branch: 'main', url: 'https://github.com/basireddym/Terraform/'
            }
        }
        stage('Terraform init'){
            steps{
                sh 'terraform init'
            }
        }
        stage('Terraform apply'){
            steps{
                sh 'terraform apply --auto-approve'
            }
        }
    }
}
