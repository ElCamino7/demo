pipeline{
  agent any

  parameters{
    gitParameter:  name: "TAG",
                    type:  "PT_TAG",
                    defaultValue: "main"
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
  
