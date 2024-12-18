---
title: "Get started with Vert.x"
cover: ../images/vertx.png
---

# Get started with Vert.x

In this guide, you’ll learn how to get started with a new Vert.x Web project.

Before starting, you need:

+ JDK 1.8 or higher
+ A text editor or IDE
+ Maven 3 or higher
+ curl or HTTPie or a browser to perform HTTP requests

## 1 Bootstrap

To create a new project, go to start.vertx.io.

Choose the version of Vert.x you want to use, choose Java as the language, Maven as the build tool, and type the group id and artifact id you want. Then, add Vert.x Web as a dependency by typing it in the “Dependencies” text box. When you’re done, hit the Generate Project button. Save the zip on your computer and unzip it in a folder of your choice.

The generated project contains:

+ The Maven build descriptor pom.xml configured to build and run your application
+ A sample Verticle and a sample test using JUnit 5
+ An editor configuration to enforce code style
+ A Git configuration to ignore files

If you want to try it now, you can download this sample project using Maven or using Gradle.

## 2 Code

Open the project in the editor of your choice and navigate to src/main/java/com/example/starter/MainVerticle.java. This source file contains a sample Verticle (the Vert.x deployment unit) that starts an HTTP server. You’re going to modify it to greet whoever performs requests to your server. Change the code as follows:
