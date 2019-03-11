pipeline {
    stages {
        stage('Deliver for development') {
            when {
                branch 'development' 
            }
            steps {
                input message: 'Finished using the web site? (Click "Proceed" to continue)'
                echo "dev"
            }
        }
        stage('Deploy for production') {
            when {
                branch 'production'  
            }
            steps {
                input message: 'Finished using the web site? (Click "Proceed" to continue)'
                echo "prod"
            }
        }
    }
}
