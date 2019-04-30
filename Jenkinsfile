node("master"){
  def String giturl = "git@github.com:ten-peb/docker-ubuntu-nodejs-8.git"
  def String clone2 = 'docker-ubuntu-nodejs-8'
  def String image_tag = "ubuntu-nodejs-8:0.5.0"
  stage("checkout source"){
    // checkout the master branch of the image repo 
    doGitClone(giturl,clone2)
  }
  stage("build image"){
    dir('docker-ubuntu-nodejs-8'){
      doDockerBuild(image_tag)
    }		 
  }
}