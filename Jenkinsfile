pipeline{
        agent any
        stages{
            stage('Make Directory'){
                steps{
                    sh "mkdir ~/thurs-2"
                }
            }
stage('git'){steps{git branch: 'main', url: 'https://github.com/cepGH1/thursday2.git'}}
stage('run shell'){steps{sh 'sh myscript.sh'}}
stage('archive'){steps{archiveArtifacts artifacts: 'output.txt', followSymlinks: false}}
            stage('Make Files'){
                steps{
                    sh "touch ~/thurs-2/file1 "
                }
            }
        }
}
