pipeline{

    agent any

// uncomment the following lines by removing /* and */ to enable
    tools{
       nodejs 'nodejs' 
    }
    

    stages{
        stage('compile-app'){
            steps{
                echo 'this is the compile-app job'
                sh 'npm install'
            }
        }
        stage('test-app'){
            steps{
                echo 'this is the test-app job'
                sh 'npm test'
            }
        }
        stage('package-app'){
            steps{
                echo 'this is the package-app job'
                sh 'npm run package'
            }
        }
    }
    
    post{
        always{
            echo 'Hi, this is my first pipeline code completed...'
        }
        
    }
    
}
