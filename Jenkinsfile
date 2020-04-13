#!groovy

def kubectlTest() {
    // Test that kubectl can correctly communication with the Kubernetes API
    echo "running kubectl test"
    sh "kubectl get nodes"

}

def helmTest() {
    // lint helm chart
    sh "/usr/local/bin/helm version"

}





node {
        stage "Testing"
        helmTest();
        kubectlTest();
        echo "Done testing"
}
