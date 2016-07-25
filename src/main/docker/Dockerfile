FROM frolvlad/alpine-oraclejdk8:slim
ADD /var/jenkins_home/jobs/Jenkins_Docker_Test/workspace/target/product-catalogue-service-1.0.jar product-catalogue-service.jar
RUN sh -c 'touch /product-catalogue-service.jar'
ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/product-catalogue-service.jar"]
