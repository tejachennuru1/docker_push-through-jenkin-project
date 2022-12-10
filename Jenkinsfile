pipeline {
    agent { label 'Jenkinsdocker' }

    stages {
        stage(vcs) {
            steps {
                git branch: 'master',
            url: 'https://github.com/DevProjectsForDevOps/StudentCoursesRestAPI'
            }
        }
    }

        stage(build) {
            steps {
                sh 'docker image build -t studentcoursesrestapi:1.0'
                sh 'docker image tag tejaaws / studentcoursesrestapi:1.0'
                sh 'docker image push'
            }
        }
}
}}}