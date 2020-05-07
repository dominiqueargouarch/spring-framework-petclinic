pipeline {
agent any
tools {
maven "Maven 3.6.3"
}
stages {
stage('jmeter') {
steps {
sh "jmeter -Jjmeter.save.saveservice.output_format=xml -Jjmeter.save.saveservice.response_data.on_error=true -n -t HTTP_Request_Defaults.jmx -l testresult.jlt"
}
}
}
}
