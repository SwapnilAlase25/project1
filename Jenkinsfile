properties([parameters([booleanParam(defaultValue: false, description: '', name: 'build_stage'), booleanParam(defaultValue: false, description: '', name: 'test_stage'), booleanParam(defaultValue: false, description: '', name: 'deloy_stage')]), pipelineTriggers([upstream('seed_repo, ')])])


node { 
    if(params.build_stage == true){
        stage('Building') {
            echo "Building project1 files"
        }
    }
    
    if(params.test_stage == true){
    stage('Testing') {
            echo "Testing project1 files" 
        }
    }
    
    if(params.deloy_stage == true){
    stage('Depolying') {
             echo "Deploying project1 files" 
        }
    }
 }
