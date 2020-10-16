## Javalin Tomcat Embed Test

Demoes embedding of [Javalin](https://javalin.io/) into the Tomcat servlet
container, without having to have Jetty on classpath.
See https://github.com/tipsy/javalin/issues/402 for more details.

To run the demo, just open your terminal and type:

```bash
git clone https://github.com/phelliperodrigues/javalin-tomcat-embed-example.git
cd javalin-tomcat-embed-example
./gradlew clean appRun
```

This will run Gradle Gretty plugin which in turn launches this WAR app in Tomcat.
When the server boots, you can access the REST endpoint simply by typing
this in your terminal, or opening http://localhost:8080/rest :

```bash
curl localhost:8080/rest/
```

It should print "Hello!".

The demo consists of only one class: [MyRestServlet.kt](src/main/kotlin/MyRestServlet.kt).
