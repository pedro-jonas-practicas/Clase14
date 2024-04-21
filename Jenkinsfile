pipeline {
    agent any

    parameters {
        string(name: 'PROCESS_NAME', defaultValue: 'bash', description: 'Nombre del proceso a buscar')
    }

    stages {
        stage('Ejecutando el Script') {
            steps {
                script {
                    sh 'chmod +x ./informe_del_sistema.sh'
                    sh "./informe_del_sistema.sh ${params.PROCESS_NAME}"
                }
            }
        }
    }
    // post {
    //     always {
    //         echo 'El job ha sido completado.'
    //     }
    // }
}
