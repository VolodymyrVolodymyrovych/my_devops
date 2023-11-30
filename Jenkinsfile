@Library("jenkins-library") _
pipeline {
    agent any
    stages {
        stage("Git Checkout") {
            steps {
                // Your Git checkout steps go here
                script {
                    // Example: Git checkout command
                    git branch: 'main', url: 'https://github.com/VolodymyrVolodymyrovych/my_devops'
                }
            }
        }

        stage("Build") {
            steps {
                // Your build steps go here
                sh "ls -lart ./*"
                sh "cat /etc/*release"
                helloWorldExternal(name:"Volodymyr", surname:"Volodymyrovych")
            }
        }

        // Add more stages as needed
    }
}
