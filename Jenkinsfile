pipeline {
  agent any
  stages {
    stage('Stage 1 ') {
      steps {
        sh 'git clone https://github.com/abesrour1111/git_devops.git'
      }
    }

    stage('Stage 2 ') {
      steps {
        sh '''ls gestion_groupes >> /dev/null 2>&1 && echo "Mon fichier existe") || echo "Mon fichier n\'existe pas"
ls  gestion_utilisateurs >> /dev/null 2>&1 && echo "Mon fichier existe") || echo "Mon fichier n\'existe pas"'''
      }
    }

  }
}