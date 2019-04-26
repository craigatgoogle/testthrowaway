/*
 * Copyright 2019 Google LLC
 *
 * Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except
 * in compliance with the License. You may obtain a copy of the License at
 *
 *     https://www.apache.org/licenses/LICENSE-2.0
 *
 * Unless required by applicable law or agreed to in writing, software distributed under the License
 * is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
 * or implied. See the License for the specific language governing permissions and limitations under
 * the License.
 */

pipeline {
    agent any
    stages {
        // stage('Build') {
        //     // Build your app
        // }
        stage('Deploy to GKE') 
        steps{
            // step([$class: 'KubernetesEngineBuilder', projectId: 'graphite-test-jenkins-ci', clusterName: 'test-cluster-foo', zone: 'us-central1-c', manifestPattern: 'manifest.yml', credentialsId: 'graphite-test-jenkins-ci'])
            step([$class: 'KubernetesEngineBuilder', projectId: 'graphite-platforms-jenkins-ci', clusterName: 'my-jenkins-cluster', zone: 'us-central1-c', manifestPattern: 'manifest.yml', credentialsId: 'graphite-platforms-jenkins-ci'])
    }
}

