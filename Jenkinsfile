pipeline{
        agent any
        stages{
            stage('Make Directory'){
                steps{
                    sh "mkdir ~/thurs-2"
                }
            }
stage('git'){steps{git branch: 'main', url: 'https://github.com/cepGH1/thursday2.git'}}
stage('run shell'){steps{sh myscript.sh}}
            stage('Make Files'){
                steps{
                    sh "touch ~/thurs-2/file1 "
                }
            }
        }
}
