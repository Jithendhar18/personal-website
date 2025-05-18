# Personal Website Template

This is a template Angular application designed for developer to customise and display their achievements and personal projects. The website that this project was based on is https://gurneetbhatia.me. You can check it out to see what the template would look like.

## Installing Angular

To run this project and be able to fully customise the UI too, you will need to install Angular and its CLI. You can follow the instructions for this on https://angular.io/guide/setup-local. If you have not already installed it, you will also need `npm` installed on your system.

## Installing node modules

Before you can get started with this project, you will have to install the necessary packages. If you are using npm, you can use `npm install` from a terminal after going into the project directory. If you prefer yarn, you can simply type `yarn` or `yarn install`.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files. If you would like to use `npm` or `yarn` to manage your project commands, you can also use `npm start` or `yarn start`.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `--prod` flag for a production build.

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI README](https://github.com/angular/angular-cli/blob/master/README.md).

## Customising the content

### The index file

### The Projects Page

```ts
export const projects: Project[]
```
```ts
id: string; // this is the route at which your project details will be stored. For example project id: "sqs" will be at localhost:4200/projects/sqs
title: string; // the title of the project displayed at the top of the project view and the project card component
description: string; // a short description of the project that is displayed in the project card component
date: string; // Can be any string that represents the date that you worked on this project
cardPhotoUrl: string; // the url or filepath at which the project cards' photo is stored
sections: Section[]; // a list of section objects that will be displayed in the project details view (defined below)
tech: string[]; // a list of the technologies that you used to build this application
projectLinks: ProjectLink[] // include any project links like GitHub repo, devpost, website,etc. relating to the project (defined below)
titlePhotoUrl?: string; // if provided, the photo displayed below the title in the project details view 
titleVideoUrl?: string; // if provided, the YouTube video below the title in the project details view
galleryImages?: GalleryImage[]; // if provided, a list of screenshots/images with descriptions relating to the project (defined below)
```

```ts
title: string;
text: string[];
```
```ts
text: string;
link: string;
```
```ts
photoUrl: string;
text?: string;
```
```ts
export const projects: Project[] = []
```
### The Competitions Page
```ts
export const competitions: Competition[]

export const competitions: Competition[]  = []
```
