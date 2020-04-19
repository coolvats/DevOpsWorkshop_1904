node{
    environment {
    registry = "coolvats/deployapp_web"
    registryCredential = 'Awaravats29@'
    }
    stage('SCM Checkout')
    {
        git 'https://github.com/coolvats/DevOpsWorkshop_1904.git'
    }
    
    stage('Run Docker Compose File')
    {
        sh '/usr/local/bin/docker-compose build'
        sh '/usr/local/bin/docker-compose down'
        sh '/usr/local/bin/docker-compose up -d'
    }
    
    stage('Push Docker Image to HUB')
    {
        sh 'docker push coolvats/deployapp_web'
    }
    
}
