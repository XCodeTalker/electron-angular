# ElectronAngular

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 17.3.0.
The purpose of this Angular project is create a exectuable.

# Set up to create a executable.

1. Use `npm install` electron' to install eletron necessary packages. Now you `pacakge.json` should have electron in your dependencies.

2. Navigate to your `index.html` and change the href for the base path to `./`. So electron will now which path it has navigate.

3. Create a `app.js` in your root folder. This will define the window on start up the executable. A example of this is create in this project.

4. Navigate back to you `package.json` and define the `app.js` as the main-class: `"main": "app.js"`. Also define under the script a two new commands
    1. `"electron": "electron .",`
    2. `"electron-build": "ng build && electron ."`

5. Now to test this you can basically just write in the terminal: `npm run electron-build` which will create the browser window with the running application

6. To have an executable you just have to install the electron-packager to by typing: `npm install @electron/packager` which will be added to your `package.json`

7. Now you can create a running executable by packing you application with the command:
    1. For Windows `npx @electron/packager ./ <name_of_your_application> --plattform-win32 --overwrite`

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The application will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via a platform of your choice. To use this command, you need to first add a package that implements end-to-end testing capabilities.

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI Overview and Command Reference](https://angular.io/cli) page.
