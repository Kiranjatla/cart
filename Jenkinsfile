pipeline{

    agent any

    stages{
        stage('Code Quality'){
          steps{
              echo 'code qaulity'
              sh 'env'
              }
          }

        stage('Style Checks'){
           when{
           branch 'master'
           }
          steps{
              echo 'Style Checks'
                    }
                }
        stage('Unit Tests'){
        when{
                   branch 'master'
                   }
          steps{
              echo 'Unit Tests'
                    }
                }
        stage('Download Dependencies'){
          when{ tag "*" }
          steps{
              echo 'Download Dependencies'
                    }
                }
        stage('Prepare Artifact'){
           when{ tag "*" }
           steps{
               echo 'Prepare Artifact'
                    }
                }
       stage('Publish Artifact'){
           when{ tag "*" }
                         steps{
                             echo 'Publish Artifact'
                    }
                }
       }

     }
