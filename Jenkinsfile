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
        sh 'gladle build'
      }
    }
    stage('test')
    {
      steps
      {
        sh 'gradle test'
      }
    }
    stage('')
    {
      steps
      {
        sh 'gradle run'
      }
    }
  }
}
