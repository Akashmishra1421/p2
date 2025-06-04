pipeline
{
  agent any
  tools
  {
    gradle 'Gradle'
    jdk 'JDK'
  }
  stages
  {
    stage('checkout')
    {
      steps
      {
        git 'https://github.com/Akashmishra1421/p2.git'
      }
    }
    stage('build')
    {
      steps
      {
        sh 'gladlew build'
      }
    }
    stage('test')
    {
      steps
      {
        sh 'gradlew test'
      }
    }
    stage('')
    {
      steps
      {
        sh 'gradlew run'
      }
    }
  }
}
