pipeline {
    agent any

    stages {
        stage ('Clonar Repositório') {
            steps {
                git branch: 'main', url: 'https://github.com/ramosjuliano/exercicio_modulo14_EBAC.git'
            }
        }
        stage ('Instalar Dependências') {
            steps {
                sh 'npm install'
            }
        }
        stage ('Executar Testes') {
            steps {
                sh 'npm run cy:run'
            }
        }
    }
}