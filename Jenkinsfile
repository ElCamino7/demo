pipeline{
  agent any

  parameters{
    choice(name: "Version", choices: ["0.0.1","0.0.2"], description : "")
    booleanParam(name: "Si", defaultValue: true, description: "")
  }
  stages{
    
    stage("Salutami"){
      steps{
      echo "Hello World"
      }
    }

    stage("Joe Pesci"){
      when{
        expression{
          params.Si == true
        }
      }
      steps{
        echo "Buffo come"
      }
    }
    
    stage("De Niro"){
      steps{
        echo "Buffo come"
        echo "Versione ${params.Version}"
      }
    }
    
  }
}
  
