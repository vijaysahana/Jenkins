pipeline {
 agent any
 stages {
 stage('Job 1') {
 steps {
 script {
echo "Starting Job 1..."
 }
 build job: 'Job 1', wait: true
 script {
 echo "Job 1 completed successfully."
 }
 // Wait for user input to continue
 input message: 'Proceed to Job 2?'
 }
 }
 stage('Job 2') {
 steps {
 script {
 echo "Starting Job 2..."
 }
build job: 'Job 2', wait: true
 script {
 echo "Job 2 completed successfully."
 }
 // Wait for user input to continue
 input message: 'Proceed to Job 3?'
 }
 }
 stage('Job 3') {
 steps {
 script {
 echo "Starting Job 3..."
 }
build job: 'Job 3', wait: true
 script {
 echo "Job 3 completed successfully."
 }
 // Final message
 echo "All jobs completed."
 }
 }
 }
}
