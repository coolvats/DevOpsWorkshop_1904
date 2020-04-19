node{

    stage('SCM Checkout')
    {
        git 'https://github.com/iamdevopstrainer/onlineshop.git'
    }
    
    stage('Run Docker Compose File')
    {
        sh '/usr/local/bin/docker-compose --versiondocker-compose build'
        sh '/usr/local/bin/docker-compose --versiondocker-compose down'
        sh '/usr/local/bin/docker-compose --versiondocker-compose up -d'
    }
    
    stage('Push Docker Image to HUB')
    {
        sh 'docker push coolvats29/deployapp_web'
    }
    
}
