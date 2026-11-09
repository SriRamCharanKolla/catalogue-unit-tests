def configMap = [
    project: "roboshop",
    component: "catalogue"
]

echo "Triggering the library pipeline"

if ( env.BRANCH_NAME.equalsIgnoreCase('main') ){
    configMap["jiraProject"] = "ROBO"
    nodeJSEKSMainPipeline(configMap)
}
else{
    configMap["jiraProject"] = "ROBO"
    nodeJSEKSPipeline(configMap)
}