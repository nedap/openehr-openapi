# OpenEHR OpenAPI code generation example

This small project demonstrates the possibilities of generating OpenEHR models and a simple API client or server stub base on automatically generated OpenAPI definitions. These definitions have been generated with https://github.com/openehr/archie .

## Build Instructions

1. Install java
2. Install gradle
3. run

```
./gradlew clean build
```

The `build/generated/src` folder will now contain the generated sources. Note that they will not automatically be considered sources to be compiled for now, merely the output.


## Changing the output format

There are many code generators available, for many languages and documentation formats. To see which ones are available, run:

```
./gradlew openApiGenerators
```

To select the generator you want, open build.gradle and set the `generatorName`-property, both for the RM and AOM