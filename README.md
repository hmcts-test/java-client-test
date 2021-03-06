# timj-onetwo

backstage docs-test

## Code generation from Swagger

Generated using [openapi-generator](https://github.com/OpenAPITools/openapi-generator)

### API updates

To update code with updated OpenAPI, [run script](./bin/code-gen.sh)

```
../bin/code-gen.sh
```

`Note : This generates a maven project and changes need to be merged manually to gradle and made sure any manual changes are not overridden`

## Building and publishing the application

### Building the library

The project uses [Gradle](https://gradle.org) as a build tool. It already contains
`./gradlew` wrapper script, so there's no need to install gradle.

To build the project execute the following command:

```bash
  ./gradlew build
```

### Publishing the library

Library automatically published to [JitPack](https://jitpack.io/#hmcts/timj-onetwo), build logs and compiled libraries can be found by going to [hmcts/timj-onetwo](https://jitpack.io/com/github/hmcts/timj-onetwo). The [Jitpack Build workflow](.github/workflows/jitpack_build.yml) will run when a tag has been created forcing JitPack to build the library so its readily available.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
