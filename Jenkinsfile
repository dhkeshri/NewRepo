
pipeline
{
    agent ("Slave Node")
    stages
    {
        stage('Full Flows')
        {
            steps
             {
                parallel(
                          first:
                          {
                            bat ''
                          },
                          second:
                          {
                            bat 'pytest .\\Pytest\\Second.py'
                          }
                      )
             }
        }
    }
}