node('maven') 
{
stage 'build'
openshiftBuild(namespace: 'development',buildConfig: 'openshift-quickstarts', showBuildLogs: 'true')
}
