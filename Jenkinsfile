pipelineJob('AwesomeBild') {

    description("A pipeline created by dsl")

    definition {

    }
}


node {


    stage('init') {

         def choice1
         def choice2

         List params = []
           
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

