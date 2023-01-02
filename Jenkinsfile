pipeline {
    agent any

    stages {
        stage('Submit Stack') {
            steps {
                sh aws cloudformation create-stack --stack-name ec2 --template-body file://ec2.yaml --parameters file://input.json --capabilities CAPABILITY_NAMED_IAM
            }
        }

    }
}
    