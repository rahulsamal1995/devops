pipeline{
    
    agent any 

    
    stages{
        stage('build') {
            steps{
               script {
                  //Ensure Maven in the PATH
                      bat 'mvn -v'  // Verify Maven installation
                      bat 'mvn clean install' // Run the Maven build
                }
            }
        }
        stage('testing') {
             steps{
                 echo "my code is getting test..."
             }
        }
        stage('code analysis') {
            steps{
                echo "my code is anyalise..."
            }
        }
        stage('deploy') {
            steps{
                echo "deploy my code..."
            }
        }
    }
