# Tutorial #

## api .Net Core console application steps ##

1. in src/api type:
```
dotnet new console
```
2. resolve dependencies:
* in Visual Studio Code there is an extension to automatically detect the need for this and do the *dotnet restore*
```
dotnet restore
```
3. run new application:
```
dotnet run
```
4. add required packages to api.csproj file
    * don't forget to change the version numbers from 1.1.0 (old dotnet versions), to 2.0
5. rewrite program.cs
6. add ContactsController.cs in src/api/Controllers
7. Run with
```
dotnet run
```
8. View in a browser pointed to *http://localhost:5000/api/contacts*


## app application with Electron and AngularJS dependencies ##

In the src/app directory:
1. create package.json file that referneces Electron and AngularJS deps
2. install the dependencies with:
```
npm install
```
3. create a *main.js* file for our entry point to the application
4. create an index.html file to correctly display the *contacts* (for this tutorial)
5. create an *app.js* file to initialize AngularJS, and have a controller which binds the data and a service to fetch data from *http://localhost:5000/api/contacts*
6. type
```
npm start
```
7. voila, the electron window pops up
