
pipeline
{
    agent "Slave Node"
    stages
    {
        stage('Full Flows')
        {
            steps
             {
                parallel(
                          first:
                          {
                            bat 'pytest .\\One\\First.py'
                          },
                          second:
                          {
                            bat 'pytest .\\One\\Second.py'
                          }
                      )
             }
        }
    }
}