node { 
    stage 'Check Out Code Repository'
        checkout scm
    stage 'build prject'
        sh 'mvn clean package'
    stage 'run prject'
        sh 'java -cp target/helloworld-1.0.jar com.coveros.demo.helloworld.HelloWorld'
    stage 'deploy to node'
        ansiblePlaybook(credentialsId: 'private_main', inventory: 'roles/inventory.ini', playbook: 'roles/main.yml')     
 }
