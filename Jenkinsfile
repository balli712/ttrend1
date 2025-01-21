pipeline{
    agent{
      node{
           label 'maven-nodes'
    }
  }
  enviorment  {
        PATH= "/opt/apache-maven-3.9.9/bin:$PATH"
  }
   stages{
      stage("build stage"){
        steps {
            sh 'mvn clean deploy'
        }
      }
   }
}