pipeline {
    agent {
        docker {
            image 'maven:3-alpine'
            args '-v C:\Users\Maheswara\.m2:C:\Users\Maheswara\.m2'
        }
    }
    stages {
        stage('Build') {
            steps {
                bat 'mvn -B -DskipTests clean package'
            }
        }
        //stage('Test') {
        //    steps {
        //        sh 'mvn test'
        //    }
        //    post {
        //        always {
        //            junit 'target/surefire-reports/*.xml'
        //        }
        //    }
        //}
        //stage('Deliver') {
        //    steps {
        //        sh './jenkins/scripts/deliver.sh'
        //    }
        //}
    }
}
