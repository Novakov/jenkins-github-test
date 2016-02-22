node {
  step([$class: 'GitHubSetCommitStatusBuilder'])

  echo 'Starting build'

  sleep(40)

  echo 'Build done'  
}

step([$class: 'GitHubCommitNotifier', resultOnFailure: 'FAILURE', statusMessage: [content: 'Build successful']])
