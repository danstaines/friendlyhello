node {
    docker.withRegistry('https://gitlab.ebi.ac.uk:5005', 'ebigitlab') {
    
        stage "build"
        def app = docker.build "friendlyhello"
    
        stage "publish"
        app.push 'master'
        app.push "banana"
    }
}