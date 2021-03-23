## Maven Calculator App
A simple calculator app I am building as I am learning Maven

### Generate a project using a Maven Archetype
```
mvn archetype:generate
```

### Compile
```bash
mvn compile
```

### Package
```bash
mvn package
```

### Install
```bash
# This packages your artifact and makes it available in your local repository
mvn install
```

### Test
```bash
mvn test
```

### Run
```
mvn exec:java -Dexec.mainClass=com.acme.App
```

### Maven strategies for dependency collisions
- Nearest definition
- First declaration

### Maven scopes
- By default, every dependency has compile scope
- "provided" scope is for compiling, but not needed to included in distributable
- "runtime" scope is the opposite of "provided" scope. something that you need to be present in runtime, but not while compile time

### Maven Lifecycles
Below is the maven default lifecycle

- validate: Validate your om.xml
- compile: Compile your project and build the classes
- test: Run tests
- package: Build a jar/war artifact
- verify: Verify your package with certain checks before installing
- install: Install it in your local mvn repository
- deploy: Deploys it to the remote repo

Running any of below lifecycle will auto run the prev ones.
For instance `mvn test` will run `validate` and `compile` before running `test`

##### Clean
The clean lifecycle removes the builds created by the project

##### site
The site lifecycle generates documentation


