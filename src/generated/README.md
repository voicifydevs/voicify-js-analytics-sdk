# Introduction 
This project includes the models and API methods for interacting with the Voicify Analytics API for JavaScript and TypeScript.

# Getting Started

You can install the package from npm:

```
npm i -s @voicify/voicify-sdk-analytics
```

If you're using TypeScript, all the types are included, so you don't need to install any additional packages.


Each service has its own API class, factory, or functional composer to use in order to make requests against it. 


Voicify Partners and Customers can also check out the extended documentation and details at https://support.voicify.com

# Build and Test
There are some steps to autogenerate the TypeScript models from the swagger API models that Voicify outputs.

## Generate Models from Swagger

Sample:

```
java -jar swagger-codegen-cli.jar generate -i http://analytics.voicify.com/swagger/v1/swagger.json -l typescript-fetch -c ../typescript-options.json -o ../../src/generated
```

## Build output

Navigate to the generated folder where the package.json is and run:

```
npm install
```

then

```
npm run build
```