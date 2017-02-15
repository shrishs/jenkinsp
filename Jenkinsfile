node('maven') 
{
stage 'build'
openshiftBuild(namespace: 'development',buildConfig: 'javaproject', showBuildLogs: 'true')
}
