pipeline {
    agent {
        label 'linux-node' // Specify the label of the node
    }
    stages {
        stage('Verify OS Type') {
            steps {
                script {
                    // Execute a script to verify the OS type
                    if (isUnix()) {
                        echo "Running on a Unix-based system"
                        sh 'uname -a' // Print detailed OS information
                    } else {
                        echo "Running on a Windows-based system"
                        bat 'ver' // Print Windows version
                    }
                }
            }
        }
        stage('Build') {
            steps {
                echo 'Executing build stage on specific node'
            }
        }
    }
}

