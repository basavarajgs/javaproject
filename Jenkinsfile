pipeline {
 agent { label 'master'}
 stages { 
   stage ('BUILD') {
     steps {
       echo "this is build stage"
     // Clean and compile the Java source code
     sh 'mvn clean compile'
     // Run tests
     sh 'mvn test'
     // Package the application
     sh 'mvn package'
      }
    }
  }
}
