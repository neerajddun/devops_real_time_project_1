pipeline {

    agent any 

    stages {

        stage ('Git Checkout') {

            steps {

                git branch: 'main', changelog: false, poll: false, url: 'https://github.com/neerajddun/devops_real_time_project_1.git'
            }
        }

        stage ('Unit Test') {

            steps {

               git 'mvn test'
            }
        }
    }
}
