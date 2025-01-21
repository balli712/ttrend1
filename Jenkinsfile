pipeline {
    agent {
        node
           {
             label 'maven-nodes'
           }
    }
environment {
    PATH = "/opt/apache-maven-3.9.9/bin:$PATH"
    MAVEN_OPTS = "-Xmx4096m"
            }
    stages {
         stage("build"){
            steps {
                 echo "----------- build started ----------"
                sh 'mvn clean deploy'
                 echo "----------- build complted ----------"
            }
        }
  }
}
