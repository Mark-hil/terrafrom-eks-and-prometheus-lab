pipeline {
    agent any

    environment {
        IMAGE_NAME = 'qr-code-app'
        TERRAFORM_DIR = 'terrafrom-eks-with-module-approach'
        AWS_REGION = 'eu-west-1'
    }

    stages {
        stage('Checkout Code') {
            steps {
                git branch: 'main', url: 'https://github.com/Mark-hil/terrafrom-eks-with-module-approach.git'
            }
        }

        stage('Terraform Version') {
            steps {
                dir("${env.TERRAFORM_DIR}") {
                    sh 'terraform -version'
                }
            }
        }

        stage('Terraform Init') {
            steps {
                dir("${env.TERRAFORM_DIR}") {
                    sh 'terraform init'
                }
            }
        }

        stage('Terraform Plan') {
            steps {
                withAWS(credentials: 'aws-cred', region: "${AWS_REGION}") {
                dir("${env.TERRAFORM_DIR}") {
                    sh 'terraform plan'
                }
            }
                
            }
        }

        stage('Terraform apply') {
            steps {
                withAWS(credentials: 'aws-cred', region: "${AWS_REGION}") {
                dir("${env.TERRAFORM_DIR}") {
                    sh 'terraform apply -auto-approve'
                }
            }
            }
        }
        stage('Terraform destroy') {
            steps {
                withAWS(credentials: 'aws-cred', region: "${AWS_REGION}") {
                dir("${env.TERRAFORM_DIR}") {
                    sh 'terraform destroy -auto-approve'
                }
            }
            }
        }
    }
}