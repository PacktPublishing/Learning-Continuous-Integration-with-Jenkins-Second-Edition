# Learning Continuous Integration with Jenkins - Second Edition
This is the code repository for [Learning Continuous Integration with Jenkins - Second Edition](https://www.packtpub.com/virtualization-and-cloud/learning-continuous-integration-jenkins-second-edition?utm_source=github&utm_medium=repository&utm_campaign=9781788479356), published by [Packt](https://www.packtpub.com/?utm_source=github). It contains all the supporting project files necessary to work through the book from start to finish.
## About the Book
In past few years, agile software development has seen tremendous growth. There is a huge demand for software delivery solutions that are fast yet flexible to numerous amendments. As a result, Continuous Integration (CI) and Continuous Delivery (CD) methodologies are gaining popularity.

This book starts off by explaining the concepts of CI and its significance in the Agile. Next, you'll learn how to configure and set up Jenkins in many different ways. The book exploits the concept of "pipeline as code" and various other features introduced in the Jenkins 2.x release to their full potential. We also talk in detail about the new Jenkins Blue Ocean interface and the features that help to quickly and easily create a CI pipeline. Then we dive into the various features offered by Jenkins one by one, exploiting them for CI and CD. Jenkins' core functionality and flexibility allows it to fit in a variety of environments and can help streamline the development process for all stakeholders. Next, you'll be introduced to CD and will learn how to achieve it using Jenkins.

Through this book's wealth of best practices and real-world tips, you'll discover how easy it is to implement CI and CD using Jenkins.

## Instructions and Navigation
All of the code is organized into folders. For example, Chapter09.



The code will look like the following:
```
node('docker') {
   stage('Poll') {
      checkout scm
   }
   stage('Build & Unit test'){
      sh 'mvn clean verify -DskipITs=true';
       junit '**/target/surefire-reports/TEST-*.xml'
       archive 'target/*.jar'
   }
```

To be able to follow everything described in the book, you will need a machine with the following configurations:

Operating systems:
     Windows 7/8/10
     Ubuntu 14 and later
Hardware requirements:
     A machine with a minimum 4 GB memory and a multicore processor
Other requirements:
    A GitHub account (public or private)

## Related Products
* [Mastering Jenkins](https://www.packtpub.com/application-development/mastering-jenkins?utm_source=github&utm_medium=repository&utm_campaign=9781784390891)

* [Continuous Delivery with Docker and Jenkins](https://www.packtpub.com/networking-and-servers/continuous-delivery-docker-and-jenkins?utm_source=github&utm_medium=repository&utm_campaign=9781787125230)

* [Effective Jenkins: Continuous Delivery with Jenkins Pipeline [Video]](https://www.packtpub.com/networking-and-servers/effective-jenkins-continuous-delivery-jenkins-pipeline-video?utm_source=github&utm_medium=repository&utm_campaign=9781788477710)
