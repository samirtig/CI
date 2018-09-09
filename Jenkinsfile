class dropDown
  {
      def static newInst(name)
      {
          def com.cwctravel.hudson.plugins.extended_choice_parameter.ExtendedChoiceParameterDefinition test =
            new com.cwctravel.hudson.plugins.extended_choice_parameter.ExtendedChoiceParameterDefinition(
              name,
              "PT_MULTI_SELECT",
              "A,B,C,D,E,F",  // displayed selection values
              null,//project name
              null,null,null,
              null,// bindings
              null,
              null, // propertykey
              "B", //default value
              null,null,null,
              null, //default bindings
              null,null,
              null, //descriptionPropertyValue
              null,null,null,null,null,null,
              null,// javascript file
              null, // javascript
              false, // save json param to file
              false, // quote
              5, // visible item count
              null,
              "," // separator
          )
          return test
  }
   }
   
node {


    stage('init') {
         List params = []
                List props = []

                Inst1 = dropDown.newInst("DDX")
                Inst2 = dropDown.newInst("DDY")

                params << booleanParam(name: 'BOOLX', defaultValue: true, description: '')
                params << Inst1
                params << Inst2

                props << parameters(params)
                properties(props)
    }

    stage('test2') {
        // Tool name from Jenkins configuration
        echo "test2"
    }

}

