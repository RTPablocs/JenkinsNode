pipeline {
  agent any
  stages {
    stage('Lint') {
      steps {
        sh '''#!/bin/bash
npm install
npm i -g eslint
eslint --fix'''
      }
    }

    stage('Test') {
      steps {
        sh '''#/bin/bash
npm i -g jest
npm test'''
      }
    }

    stage('deploy') {
      steps {
        sh '''#/bin/bash
npm run'''
      }
    }

  }
}