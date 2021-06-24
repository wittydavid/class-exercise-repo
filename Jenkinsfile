properties([parameters([string(defaultValue: 'david', name: 'NAME', trim: true)]), pipelineTriggers([pollSCM('* * * * *')])])
node {
    stage("one"){
        git branch: 'main', url: 'https://github.com/wittydavid/class-exercise-repo.git'
        sh "echo 'Hello ${env.NAME} - this is master branch build'"
        sh "cat 1.txt"
    }
}
