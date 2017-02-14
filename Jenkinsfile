node('agent') 
{
stage 'build'
openshiftBuild(namespace: 'development', buildConfig: 'javaproject', showBuildLogs: 'true')
##stage 'deploy'
##openshiftDeploy(deploymentConfig: 'frontend')
}
