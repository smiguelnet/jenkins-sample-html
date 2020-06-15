#!groovy

void printLineSep(String title) {
    echo "=================================="
    if (title != null) {
        echo "${title}"
        echo " "
    }
}

node {
    def scmVars = checkout scm

    stage('Set-PATH') {
        def mavenHome = tool 'M3'
        def dockerHome = tool 'DOCKER'
        def nodeHome = tool 'NODEJS'
        env.PATH = "${dockerHome}/bin:${mavenHome}/bin:${nodeHome}/bin:${env.PATH}"

        printLineSep("PATHS")
        echo "${env.URL_SERVER_CONSUL}"
        echo "${env.BRANCH_NAME}"
        echo "${env.GIT_BRANCH}"
    }

    stage('Report') {
        
    }

    //}
}
