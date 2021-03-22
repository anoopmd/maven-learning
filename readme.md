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

### Maven strategies for dependency collisions
- Nearest definition
- First declaration

### Maven scopes
- By default, every dependency has compile scope
- "provided" scope is for compiling, but not needed to included in distributable
- "runtime" scope is the opposite of "provided" scope. something that you need to be present in runtime, but not while compile time

