pipeline{
  agent any
    tools{
      gradle "Gradle"
      jdk "JDK"
    }
    stages{
      stage('checkout'){
        steps{
          git 'https://github.com/Gekkorizz/MyGradleProject.git'
        }
      }
      stage('build'){
        steps{
          sh './gradlew build'
        }
    }
      stage('run'){
        steps{   
          sh './gradlew run'
        }
      }
}
}
