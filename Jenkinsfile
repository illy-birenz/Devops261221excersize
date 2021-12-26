properties([pipelineTriggers([pollSCM('* * * * *')])])
node{
    stage("exersize"){
        checkout([$class: 'GitSCM', branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/illy-birenz/Devops261221excersize.git']]])
    }
    stage("show files")
    bat "dir"
}
