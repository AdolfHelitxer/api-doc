pipeline {
  agent any
  stages {
    stage('检出') {
      steps {
        checkout([
          $class: 'GitSCM',
          branches: [[name: GIT_BUILD_REF]],
          userRemoteConfigs: [[
            url: GIT_REPO_URL,
            credentialsId: CREDENTIALS_ID
          ]]])
        }
      }
      stage('发布 API 文档') {
        steps {
          codingReleaseApiDoc(apiDocId: API_DOC_ID, apiDocType: API_DOC_TYPE, resultFile: "api.json")
        }
      }
    }
  }