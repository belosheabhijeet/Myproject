pipeline {
   agent Slave
   tools {
      maven 'M2_HOME'
stages {
  stage{'Checkout from Github'} {
    steps {
      git branch: 'master', url: 'https://github.com/belosheabhijeet/Myproject.git'
          }
  }
  stage{'Build using maven'} {
    steps {
      sh 'mvn clean package'
    }
  }
  stage {'Echo my job'}
  steps {
    echo 'Welcome to my project'
  }
}
   }
