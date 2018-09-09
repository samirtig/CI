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
             job('example') {
                 parameters {
                     activeChoiceParam('CHOICE-1') {
                         description('Allows user choose from multiple choices')
                         filterable()
                         choiceType('SINGLE_SELECT')
                         groovyScript {
                             script('["choice1", "choice2"]')
                             fallbackScript('"fallback choice"')
                         }
                     }
                 }
             }
                List props = []

                Inst1 = dropDown.newInst("DDX")
                Inst2 = dropDown.newInst("DDY")

                params << booleanParam(name: 'BOOLX', defaultValue: true, description: '')
                params << Inst1
                

                props << parameters(params)
                properties(props)
    }

    stage('test2') {
        // Tool name from Jenkins configuration
        echo "test2"
    }

}

