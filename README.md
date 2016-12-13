# myWiki (claudePlos)


###Node (angularjs with server)
New folder (name project) and add in
package.json
```sh
{
  "name": "angular-quickstart",
  "version": "1.0.0",
  "scripts": {
    "start": "tsc && concurrently \"tsc -w\" \"lite-server\" ",
    "lite": "lite-server",
    "tsc": "tsc",
    "tsc:w": "tsc -w"
  },
  "licenses": [
    {
      "type": "MIT",
      "url": "https://github.com/angular/angular.io/blob/master/LICENSE"
    }
  ],
  "dependencies": {
    "@angular/common": "~2.1.1",
    "@angular/compiler": "~2.1.1",
    "@angular/core": "~2.1.1",
    "@angular/forms": "~2.1.1",
    "@angular/http": "~2.1.1",
    "@angular/platform-browser": "~2.1.1",
    "@angular/platform-browser-dynamic": "~2.1.1",
    "@angular/router": "~3.1.1",
    "@angular/upgrade": "~2.1.1",
    "angular-in-memory-web-api": "~0.1.13",
    "bootstrap": "^3.3.7",
    "core-js": "^2.4.1",
    "reflect-metadata": "^0.1.8",
    "rxjs": "5.0.0-beta.12",
    "systemjs": "0.19.39",
    "zone.js": "^0.6.25"
  },
  "devDependencies": {
    "@types/core-js": "^0.9.34",
    "@types/node": "^6.0.45",
    "concurrently": "^3.0.0",
    "lite-server": "^2.2.2",
    "typescript": "^2.0.3"
  }
}
```
in command line npm install and add in folder project secound file name: server.js
```sh
var http = require('http'),
    fs = require('fs');


fs.readFile('./index.html', function (err, html) {
    if (err) {
        throw err;
    }
    http.createServer(function(request, response) {
        response.writeHeader(200, {"Content-Type": "text/html"});
        response.write(html);
        response.end();
    }).listen(8000);
});
```
and in command line node server.js (http://localhost:8000/)
###TypeSript
```sh
npm install -g typescript
```
In your editor, type the following JavaScript code in greeter.ts
```sh
tsc greeter.ts   
```
more info: [TS](https://www.typescriptlang.org/docs/tutorial.html)

###GitHub
.gitconfig
add in home directory project file directory and add path to file no send to git
```sh
/node_modules/*
```


###AngularJS
ngController
https://docs.angularjs.org/api/ng/directive/ngController
 
ng-repeat --> loop 

ng-model --> MVVM, 2 way data binding



###Java
stream :) Java8
```
for ( StanZywionychMMRapRozDTO rr : stanZywionychRapRoz )
{
  if( stanZywionychRapRoz2.stream().anyMatch( p -> p.getGz().equals(rr.getGz())) )
  {
      StanZywionychMMRapRozDTO firstMatchedName = stanZywionychRapRoz2.stream()
            .filter((s) -> s.getGz().equals(rr.getGz() ))
            .findFirst().get();
  }
}

or 

boolean check = stanZywionychRapRoz2.stream().anyMatch( p -> p.getGz().equals(rr.getGz()));

```                     
                      
                      

###CSS
z-index

###ORACLE
Tnsnames.org -> FAILOVER_MODE = (TYPE=SELECT)(METHOD=BASIC).... 


###FinTech

###Refaktoring
###SAGI
###LEGACY CODE - EFEKTYWNA REWITALIZACJA



HBOX ---

VBOX<br>
|<br>
|<br>
|<br>
