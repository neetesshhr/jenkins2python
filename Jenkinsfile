node{
    stage('checkout source'){
        echo "checking out source ..."
        checkout scm
    }
    stage('parameters building '){
        properties([
            parameters([
                string(name:'username', defaultValue:'Nitesh Rijal', description: 'Enter username')
            ])
        ])
    }
    stage('build the python file'){
        bat ''' python index.py'''
    }
}