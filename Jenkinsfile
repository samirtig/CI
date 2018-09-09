node {
    properties([
         parameters([
           booleanParam(
             defaultValue: false,
             description: 'isFoo should be false',
             name: 'isFoo'
           ),
           booleanParam(
             defaultValue: true,
             description: 'isBar should be true',
             name: 'isBar'
           ),
         ])
       ])

    stage('test1') {
        echo "ok"
    }

    stage('test2') {
        // Tool name from Jenkins configuration
        echo "test2"
    }

}

