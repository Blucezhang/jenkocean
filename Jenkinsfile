pipeline {
  agent any
  stages {
    stage('git clone') {
      steps {
        git(url: 'git clone https://github.com/Blucezhang/jenkocean.git', branch: 'dev', changelog: true)
      }
    }
    stage('mvn ') {
      steps {
        sh '''#!/bin/bash

mvn clean install'''
      }
    }
  }
}