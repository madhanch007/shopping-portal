pipeline{

    agent any

// uncomment the following lines by removing /* and */ to enable
   tools{
       nodejs 'nodejs' 
    }
    

    stages{
        stage('compile-app'){
            steps{
                echo 'this is the compile job'
                sh 'npm install'
                sleep 4
            }
        }
        stage('test-app'){
            steps{
                echo 'this is the test job'
                sh 'npm test'
                sleep 9
            }
        }
        stage('package-app'){
            steps{
                echo 'this is the package job'
                sh 'npm run package'
                sleep 7
            }
        }
    }
    
    post{
        always{
            echo 'this is the first pipeline...'
        }
        
    }
    
}
