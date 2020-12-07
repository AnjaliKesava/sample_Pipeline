pipeline {
    agent any
        stages {
            stage('Compile') {
                steps{
                    echo "compiled successfully";
                }
            }
            stage('JUnit') {
                steps{
                    echo "JUnit passed successfully";
                }
            }
            stage('Quality gate') {
                steps{
                    echo "Qulity gate passed successfully";
                }
            }
            stage('Deploy') {
                steps{
                    echo "Passed";
                }
            }
        }
        
        post{
            always {
                echo "This will run always"
            }
            
            success {
                echo "This will run only if success"
            }
            failure {
                echo "This will run only if failed"
            }
            
            unstable {
                echo "This will run only if the run is marked as unstable"
            }
            
            changed {
                echo "This will run only if the state of the pipeline has changed"
            }
            
        }
    }
