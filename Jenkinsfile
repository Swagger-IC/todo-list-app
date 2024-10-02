node {
    stage('Preparation') {
        catchError(buildResult: 'SUCCESS') {
            sh 'docker stop todo-list-running'
            sh 'docker rm todo-list-running'
        }
    }
      stage('Build') {
        build 'buildTodoListApp'
    }
}
