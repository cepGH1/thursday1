pipeline{
        agent any
        stages{
     
stage('git'){steps{git branch: 'main', url: 'https://github.com/cepGH1/thursday2.git'}}
stage('run shell'){steps{sh 'sh myscript.sh'}}
stage('archive'){steps{archiveArtifacts artifacts: 'output2.txt', followSymlinks: false}}
            
        }
}
