node{
    checkout scm
    stage("run security scan"){
      sh "sudo docker run --network=bundlev2_prodnetwork --rm -t owasp/zap2docker-stable zap-baseline.py -t http://localhost:10000/ -u https://github.com/nks0991/oss-zap/blob/master/config"
    }
}
