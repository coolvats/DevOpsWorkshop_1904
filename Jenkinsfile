node{
    
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
    
    
    
}
