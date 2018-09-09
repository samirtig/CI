import com.cwctravel.hudson.plugins.extended_choice_parameter.ExtendedChoiceParameterDefinition
node {

    def multiSelect= new ExtendedChoiceParameterDefinition("name",
                "PT_MULTI_SELECT",
                "blue,green,yellow,blue",
                "project name",
                "",
                "",
                "",
                "",
                "",
                "",
                "",
                "",
                "",
                "",
                "",
                "",
                "",
                "blue,green,yellow,blue",
                "",
                "",
                "",
                "",
                "",
                "",
                "",
                "",
                false,
                false,
                3,
                "multiselect",
                ",")

    stage('init') {
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
                            choice(
                                    choices: "US-EAST-1\nUS-WEST-2",
                                    description: 'What AWS region?',
                                    name: 'region'
                            ),
                    ])
            ])
    }

    stage('test2') {
        // Tool name from Jenkins configuration
        echo "test2"
    }

}

