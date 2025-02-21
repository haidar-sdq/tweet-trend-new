pipeline{
    agent{
        label "maven"
    }
    environment{
        PATH = "/opt/apache-maven-3.8.8/bin:$PATH"
    }
    stages{
        stage("build"){
            steps{
                echo "========executing build========"
                sh 'mvn clean deploy'
            }
        }
    }
}