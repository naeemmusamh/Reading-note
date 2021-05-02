# express

1. What’s the difference between PUT and PATCH?

PUT means replace the entire resource with given data.

PATCH means replace only specified fields.

For the Table API, however, PUT and PATCH mean the same thing.

2. Provide links to 3 services or tools that allow you to “mock” an API for development like json-server?

A- Nock

is an HTTPS library designed to replicate and mock servers and expectations in Node.js.

B- MockServer

is a multifaceted tool that comes in a variety of builds.

C- Beeceptor

is a great tool largely because it requires absolutely no code in order to utilize it.

3. Compare and contrast Swagger and APIDoc.js 1 Which HTTP status codes should be sent with each type of (un)successful API call?

swagger-ui is meant for consumption by JavaScript web projects that include module bundlers, such as Webpack, Browserify, and Rollup. Its main file exports Swagger UI's main function, and the module also includes a namespaced stylesheet at swagger-ui/dist/swagger-ui.css.

import SwaggerUI from 'swagger-ui'
// or use require if you prefer
const SwaggerUI = require('swagger-ui')
SwaggerUI({
  dom_id: '#myDomId'
})

const express = require('express')
const pathToSwaggerUi = require('swagger-ui-dist').absolutePath()
const app = express()
app.use(express.static(pathToSwaggerUi))
app.listen(3000)

var SwaggerUIBundle = require('swagger-ui-dist').SwaggerUIBundle
const ui = SwaggerUIBundle({
    url: "https://petstore.swagger.io/v2/swagger.json",
    dom_id: '#swagger-ui',
    presets: [
      SwaggerUIBundle.presets.apis,
      SwaggerUIBundle.SwaggerUIStandalonePreset
    ],
    layout: "StandaloneLayout"
  })

docker pull swaggerapi/swagger-ui
docker run -p 80:8080 swaggerapi/swagger-ui

docker run -p 80:8080 -e SWAGGER_JSON=/foo/swagger.json -v /bar:/foo swaggerapi/swagger-ui

<script src="https://unpkg.com/swagger-ui-dist@3/swagger-ui-bundle.js" charset="UTF-8"></script>
<!-- `SwaggerUIBundle` is now available on the page -->

4. Compare and contrast SOAP and ReST?

SOAP and REST both allow you to create your own API. API stands for Application Programming Interface. It makes it possible to transfer data from an application to other applications. An API receives requests and sends back responses through internet protocols such as HTTP, SMTP, and others.

The SOAP is a standardized protocol that sends messages using other protocols such as HTTP and SMTP. 

The REST architecture lays down a set of guidelines you need to follow if you want to provide a RESTful web service.