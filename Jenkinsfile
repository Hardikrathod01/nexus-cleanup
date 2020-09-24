String taskId = "b6831d96-e233-4544-be23-678ce1e09d58"

node("${env.node}") {
  stage("Trigger Nexus Task") {
    def response = httpRequest authentication: 'nexuscreds',
    httpMode: 'POST', consoleLogResponseBody: true,
    url: "http://34.232.66.146:8081/service/rest/v1/tasks/${taskId}/run"
  } 
}
