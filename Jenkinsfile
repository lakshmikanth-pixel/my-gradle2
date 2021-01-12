pipeline {
    agent any

    stages {
        stage ('Compile Stage') {

            steps {
                withGradle(gradle : 'Gradle') {
                    sh 'gradle clean build'
                }
            }
        }

        stage ('Testing Stage') {

            steps {
                withGradle(gradle : 'Gradle') {
                    sh 'gradle test'
                }
            }
        }


    }
}
