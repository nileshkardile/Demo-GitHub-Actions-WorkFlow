# Demo-GitHub-Actions-WorkFlow
The first main.yml performs the following CI action:
  checkout the source code in workspace and create a new_tag as an output. This will be run as an dry-run at the moment.
  mvn compile - take the compiled code and package it in its distributable format, such as a JAR.
  mvn deploy - copies the final package to the github remote repository for sharing with other developers and projects.
The second create-release.yaml performs the following CD action:
  create release based on pushing tags.
