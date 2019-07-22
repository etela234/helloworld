node { 
    stage 'build prject'
        sh 'mvn clean package'
    stage 'run prject'
        sh 'java -cp target/helloworld-1.0.jar com.coveros.demo.helloworld.HelloWorld'
 }
