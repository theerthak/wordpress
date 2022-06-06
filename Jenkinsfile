pipeline{
    agent any
        stages{
            stage('clone'){
               steps{
                   script{
                       git credentialsId: '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', url: 'https://github.com/theerthak/wordpress.git'
                   }
               }
            }
            stage('deploy'){
                steps{
                    script{
                        '''docker-compose up -d'''
                    }
                }
            }
        }
  }
