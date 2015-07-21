Installs plugins:
  * AWS CodeDeploy
  * AWS CodePipeline
  * SBT
  * Cloudbees Docker "Build and Publish" 
  * various dependencies
Based on official Jenkins image. See `https://registry.hub.docker.com/_/jenkins/ and https://github.com/jenkinsci/docker`.

In order to allow Docker plugin to run within Jenkins,

`docker run -p 8080:8080 -v /var/run/docker.sock:/var/run/docker.sock -v /home/local-user/jenkins:/var/jenkins_home zenchicken/jenkins-codepipeline`
