pipeline {
  
    agent any
    
    tools{
        maven "M2_HOME"
    }

    stages {
        stage('Clone') {
            steps {
               git 'https://github.com/ashokitschool/maven-web-app.git'
            }
        }
        stage('Build') {
            steps {
               sh 'mvn clean package'
            }
        }
        
        /* stage('Create Image'){
            steps{
               steps {
                	script {
                		sh 'ansible-playbook task.yml'
                	}
                }
            }
        } */
    }
}
