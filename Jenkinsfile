pipeline
{
    agent any
    environment
    {
         tiempo_actual = "Soleado"
    }
    stages
    {
        stage("-------")
        {
            steps
            {
                script
                {
                    def dia = new Date().getDay()
                    
                    if (dia == 1)
                    {
                        println "No hacemos nada"
                    }
                    else if (dia == 2)
                    {
                        echo "El usuario de ejecución es ${env.USERNAME}"
                    }
                    else if (dia == 3)
                    {
                        println "El tiempo actual es: "+soleado
                    }
                    else if (dia == 4)
                    {
                        git branch: "main", url: "https://github.com/xavicolmenero/CICD_Jenkins.git"
                    }
                    else if (dia==5)
                    {
                        println "No hacemos nada"
                    }
                }
            }
        }
    }
}
