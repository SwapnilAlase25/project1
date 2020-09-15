properties([parameters([booleanParam(defaultValue: true, description: '', name: 'build_stage'), booleanParam(defaultValue: true, description: '', name: 'test_stage'), booleanParam(defaultValue: true, description: '', name: 'deloy_stage')]), pipelineTriggers([upstream('seed_repo, '),cron('H * * * *')])])


node {
    try{
        if(params.build_stage == true){
            stage('Building') {
                echo "Building project1 files"
            }
        }
    }catch(e){
     echo "Build Failed!"   
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
