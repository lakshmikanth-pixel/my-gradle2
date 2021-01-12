pipeline {
    agent any

    stages {
        stage ('Compile Stage') {

            steps {
                withgradle(gradle : 'Gradle') {
                    sh 'gradle build'
                }
            }
        }

        stage ('Testing Stage') {

            steps {
                withgradle(gradle : 'Gradle') {
                    sh 'gradle test'
                }
            }
        }


    }

}
