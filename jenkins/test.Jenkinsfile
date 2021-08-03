pipeline {
    agent any
    parameters {
    string(defaultValue: "Test" ,description:"Which environment to deploy ?",name:"deployenv")
    choice(choices:["EU-WEST-2A","EU-WEST-2B","EU-WEST-2C"],description:"Select which az to deploy to",name:"deployaz")
    booleanParam(defaultValue:"false",description:"Start deployment",name:"deploycheck")

    }
    stages{
        stage("Demo"){
         steps{
             echo "Deployment variable is set to :${params.deployenv}"
             echo "Deployment availability zone:${params.deployaz}"
             echo "Deployment availability zone:${params.deploycheck}"
              }
        }
    }
}
