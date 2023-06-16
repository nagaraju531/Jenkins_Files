pipeline {
    agent {
    node {
      label 'linux'
    }
  }
    stages {
        stage('CheckOut the Code') {
            steps {
                echo "Hello World"
                //sh "checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'github', url: 'https://github.com/nagaraju531/ansible_playbooks']])"
                git credentialsId: 'github', url: 'https://github.com/nagaraju531/ansible_playbooks'
        }
    }
       state("Check Syntax Check"){
               steps {
			      dir('/var/lib/jenkins/workspace/Ansible_Tower_PipeLine') {
                   ansible-lint main.yml
}
}
}
}
}
