The easiest way to get started with **svyAPI** is to download and import the *.servoy file of the example solution **svyAPIExample**. It includes everything needed to get you going:

* the core module svyAPI
* the example solution svyAPIExample which provide samples samples how to use the jsdoc anotation.

Additional you need to download Swagger UI what can be found [here](https://github.com/swagger-api/swagger-ui/releases).

After downloading the zip file follow the steps:
* Unzip the source code zip from Swagger UI
* Copy the `dist` folder to `%%servoy_developer%%/application_server/server/webapps/ROOT.
* You can rename this folder to a matching name, for example API.
* Edit the `index.html` file, search for `https://petstore.swagger.io/v2/swagger.json` end replace the url to match your `servoy_developer` url. Example `http://localhost:8080/servoy-service/rest_ws/svyAPIExample/docs/swagger.json`