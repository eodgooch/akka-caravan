scala-starter
=============

scala starter template for when working on new projects
Structure taken from: http://www.bks2.com/blog/2013/02/23/zero-to-a-scala-sbt-project/

sbt makes life much easier in a scala project. I suggest using Sublime Text for smaller projects, IntelliJ for larger (just for intellisense). The website listed above has instructions on setting up IntelliJ.

I also added in a dependency for sbt one-jar run command. This packages everything into an executable jar file to run anywhere. The run script calls the command line for specific memory configs, but you can change that.

As long as there is a singleton class under src/main/scala, sbt will find it. All other classes can be added, but this is the entry point. 

If you change the project name, reflect the changes in the run script and build.sbt

Example usage: sbt one-jar && ./run.sh
