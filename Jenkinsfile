import com.cwctravel.hudson.plugins.extended_choice_parameter.ExtendedChoiceParameterDefinition
node {

    def multiSelect= new ExtendedChoiceParameterDefinition(
            "name",
            "PT_CHECKBOX",
            "VALUE, A, B",
            null,//project name
            null,
            null,
            null,
            null,// bindings
            null,
            null, // propertykey
            "VALUE, B", //default value
            null,
            null,
            null,
            null, //default bindings
            null,
            null,
            null, //descriptionPropertyValue
            null,
            null,
            null,
            null,
            null,
            null,
            null,// javascript file
            null, // javascript
            false, // save json param to file
            false, // quote
            2, // visible item count
            "DESC",
            ","
        )

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
                            multiSelect,
                    ])
            ])
    }

    stage('test2') {
        // Tool name from Jenkins configuration
        echo "test2"
    }

}

