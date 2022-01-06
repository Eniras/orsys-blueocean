pipeline {
  agent any
  stages {
    stage('Stage 1 ') {
      steps {
        sh 'git clone https://github.com/abesrour1111/git_devops.git /var/lib/jenkins/depotjenkins'
      }
    }

    stage('Stage 2 ') {
      steps {
        sh '''ls gestion_groupes >> /dev/null 2>&1 && echo "Mon fichier existe" || echo "Mon fichier n\'existe pas"
ls  gestion_utilisateurs >> /dev/null 2>&1 && echo "Mon fichier existe" || echo "Mon fichier n\'existe pas"'''
      }
    }

    stage('Stage 3') {
      steps {
        sh '''if test ls /var/lib/jenkins/depotjenkins| wc \' -eq 2
then
grep -A1 modification gestion_groupes && grep -A1 modifications
else
echo "message d\'erreur, clone "échoué"
fi'''
      }
    }

  }
}