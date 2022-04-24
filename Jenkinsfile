pipeline {
    agent any
    tools {nodejs "my_nodejs"}
    stages {
        stage('Dev') {
            steps {
               git 'https://github.com/vivekmankar26/aws_codebuild_codedeploy_nodeJs_demo.git'
               echo "the content as follows"
               sh 'cat index.js'
            }
        }
        stage('build') {
            steps {
               sh 'npm install'
            }
        }
    }
}