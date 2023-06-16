pipeline {
    agent {
    node {
      label 'linux'
    }
  }
    stages {
        stage('CheckOut the Code') {
            steps {
                // Get some code from a GitHub repository
                echo "Hello World"
                git branch: 'main', credentialsId: 'github', url: 'https://github.com/nagaraju531/ansible_playbooks'
           }
        }
    }
}
