node {
    parameters {
            string(defaultValue: "TEST", description: 'What environment?', name: 'userFlag')
            choice(choices: ['US-EAST-1', 'US-WEST-2'], description: 'What AWS region?', name: 'region')
        }

    stage('test1') {
        echo "ok"
    }

    stage('test2') {
        // Tool name from Jenkins configuration
        echo "test2"
    }

}

