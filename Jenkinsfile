class dropDown
  {
      def static newInst(name)
      {
          def com.cwctravel.hudson.plugins.extended_choice_parameter.ExtendedChoiceParameterDefinition test =
            new com.cwctravel.hudson.plugins.extended_choice_parameter.ExtendedChoiceParameterDefinition("name",
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
          return test
  }
   }

node {


    stage('init') {

         def choice1
         def choice2

         List params = []
              def dd = [
                              $class              : 'ParametersDefinitionProperty',
                              parameterDefinitions: [
                                      [
                                              $class     : 'ChoiceParameterDefinition',
                                              choices    : 'aaa\nbbb',
                                              description: 'select your choice : ',
                                              name       : 'choice1'
                                      ],
                                      [
                                              $class     : 'ChoiceParameterDefinition',
                                              choices    : 'ccc\nddd',
                                              description: 'select another choice : ',
                                              name       : 'choice2'
                                      ]]]
                List props = []

                Inst1 = dropDown.newInst("DDX")
                Inst2 = dropDown.newInst("DDY")

                params << booleanParam(name: 'BOOLX', defaultValue: true, description: '')
                params << Inst1
                params << dd

                props << parameters(params)
                properties(props)
    }

    stage('test2') {
        // Tool name from Jenkins configuration
        echo "test2"
    }

}

