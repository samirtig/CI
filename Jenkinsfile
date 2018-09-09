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
         choice1 = input( id: 'userInput', message: 'Select your choice', parameters: [ [$class: 'ChoiceParameterDefinition', choices: 'aa\nbb', description: '', name: ''] ])
         if(choice1.equals("aa")){
             choice2 = input( id: 'userInput', message: 'Select your choice', parameters: [ [$class: 'ChoiceParameterDefinition', choices: 'yy\nww', description: '', name: ''] ])
         }else{
            choice2 = input( id: 'userInput', message: 'Select your choice', parameters: [ [$class: 'ChoiceParameterDefinition', choices: 'gg\nkk', description: '', name: ''] ])
         }
         List params = []
                List props = []

                Inst1 = dropDown.newInst("DDX")
                Inst2 = dropDown.newInst("DDY")

                params << booleanParam(name: 'BOOLX', defaultValue: true, description: '')
                params << choice1
                params << choice2

                props << parameters(params)
                properties(props)
    }

    stage('test2') {
        // Tool name from Jenkins configuration
        echo "test2"
    }

}

