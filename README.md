AngularJS Dashboard Template - EscobarMiranda.com  
===================  

> **Description:**  

> - AngularJS application  

Examples  
-------------  

Login:  
![Login](https://raw.githubusercontent.com/kescobar-pernix/angularjs-dashboard-template/master/examples/login.png)

Login:  
![Dashboard](https://raw.githubusercontent.com/kescobar-pernix/angularjs-dashboard-template/master/examples/dashboard.png)

Login:  
![Admin](https://raw.githubusercontent.com/kescobar-pernix/angularjs-dashboard-template/master/examples/admin.png)

Styleguide  
-------------  

Refer to AngularJS John Papa Styleguide: https://github.com/johnpapa/angular-styleguide  

Set Up  
-------------  
NPM and bower have to be installed in order to set up the project.  

Run bower and npm to get all dependencies needed.  
```sh  
  npm install  
  bower install  
```  

Syntax  
-------------  
Run `gulp review`  

Adding a new library  
-------------

When installing a new library with bower or npm, add it to the array in the gulp task `build-index` and also in respective task `move-bower-components`or `move-node-modules`.
The gulp file is located in the root of the project.

Build & development  
-------------  
For running the app use `gulp run` this will run the following tasks:
* `clean-less`  
* `less`  
* `build-index`  
* `review`  
* `grunt-serve`  

This will generate a general file to handle the css, which is located in app -> assets -> styles -> gash.css

- Open url  
`http://localhost:3000/`  

Adding new library  
-------------  
Whe adding new library with either npm or bower use the `--save` or `--save-dev` option.
Also add the new file's path to the gulp task `build-index` in the sources array specifically.
Then run the following command to inject those files into the index `gulp build-index`

Testing  
-------------  
Running `grunt test` will run the unit tests with karma.

----------
[![EscobarMiranda.com](http://escobarmiranda.com/EscobarMirandaLogoLittle.png)](http://EscobarMiranda.com)