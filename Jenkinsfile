node('maven') 
{
stage 'build'
openshiftBuild(namespace: 'development',buildConfig: 'openshift-quickstarts', showBuildLogs: 'true')
stage 'deploy to testing'
   input message: "Promote to STAGE?", ok: "Promote"
openshiftTag(namespace: 'development', sourceStream: 'openshift-quickstarts', sourceTag: 'latest', destinationNamespace: 'testing',destinationStream: 'openshift-quickstarts', destinationTag: 'promoteQA')
}
