pipeline {
    agent any


    stages {
        
        stage('Test') {
            steps {
                sh '''
                    
                    sudo su
                    su jenkins
                    ssh jenkins@20.77.125.95
                    sudo apt install openjdk-17-jre-headless
                    sudo timeshift --restore --snapshot '2023-09-16_21-33-53' --target /dev/sda1
                    java --version'''
            }
        }
    }
}
