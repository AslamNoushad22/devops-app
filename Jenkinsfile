pipeline {
agent any

```
stages {
    stage('Checkout') {
        steps {
            echo 'Repository checkout successful'
        }
    }

    stage('Build') {
        steps {
            echo 'Build stage running'
        }
    }

    stage('Test') {
        steps {
            echo 'Test stage running'
        }
    }
}

post {
    success {
        echo 'Pipeline completed successfully!'
    }
    failure {
        echo 'Pipeline failed. Check the console output.'
    }
}
```

}
