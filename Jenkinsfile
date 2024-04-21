pipeline {
    agent any

    parameters {
        string(name: 'PROCESS_NAME', defaultValue: 'Elimine esto y escriba el proceso a buscar...', description: 'Nombre del proceso a buscar')
    }

    stages {
        stage('Ejecucion del Script') {
            steps {
                script {
                    sh 'chmod +x ./informe_del_sistema.sh'
                    sh "./informe_del_sistema.sh ${params.PROCESS_NAME}"
                }
            }
        }
    }
}
