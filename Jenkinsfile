pipeline {
    agent any 
    stages {
        stage ('installing Jboss on Jboss-server') {
            steps {
                ansiblePlaybook credentialsId: 'JBOSS-KEY', disableHostKeyChecking: true, installation: 'Ansible', inventory: 'Jbosshosts.inv', playbook: 'Jboss.yml'
              }
        }
    }
}