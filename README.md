<h1 align="center">
NGX-FIREBASE-CMS
</h1>

<div align="center">
🛑🛑UNDER DEVELOPMENT 🛑🛑
</div>

<div align="center">
🛑 DONT USE 🛑
</div>

<div align="center">
Angular Content Management System using Google Firebase (Authentication, Storage &amp; Firestore)

[![GitHub Release Date](https://img.shields.io/github/release-date/AppQuick/ngx-firebase-cms.svg?style=flat-square)](https://github.com/AppQuick/ngx-firebase-cms/releases)
[![npm package](https://img.shields.io/npm/v/ngx-firebase-cms.svg?style=flat-square)](https://www.npmjs.org/package/ngx-firebase-cms)
[![NPM downloads](http://img.shields.io/npm/dm/ngx-firebase-cms.svg?style=flat-square)](https://npmjs.org/package/ngx-firebase-cms)
[![GitHub license](https://img.shields.io/npm/l/ngx-firebase-cms.svg?style=flat-square)](https://github.com/AppQuick/ngx-firebase-cms/blob/master/LICENSE)

</div>

## Description
`ngx-firebase-cms` is a set of tool that combines the admin panel using `ng-zorro-antd` and backend linkage to Google Firebase with what developers need for their Angular project. It provides user authentication, file storage and firestore database using Google Firebase.

## Features
- User Authentication using Firebase Authentication
- Media upload using Firebase Storage
- Post CRUD using Firebase Firestore
- Admin Panel using `ng-zorro-antd`

## Environment Support
- Angular `^7.0.0`
- Modern browsers and Internet Explorer 11+ (with [polyfills](https://angular.io/guide/browser-support))

## Installation
### 1. Create a new project
```
ng new <project-name>
cd <project-name>
```

### 2. Install NGX-FIREBASE-CMS
```
npm i -S ngx-firebase-cms
```

### 3. Add Firebase config to environments variable
Open `/src/environments/environment.ts` and add your Firebase configuration. You can find your project configuration in the [Firebase Console](https://console.firebase.google.com/). From the project overview page, click Add Firebase to your web app.
```
export const environment = {
  production: false,
  ngxFirebaseCms: {
    firebase: {
        apiKey: '<your-key>',
        authDomain: '<your-project-authdomain>',
        databaseURL: '<your-database-URL>',
        projectId: '<your-project-id>',
        storageBucket: '<your-storage-bucket>',
        messagingSenderId: '<your-messaging-sender-id>'
    }
  }
};
```
### 4. Setup @NgModule for the NgxFirebaseCmsModule
Open `/src/app/app.module.ts`, inject the NgxFirebaseCms providers, and specify your NgxFirebaseCms configuration.
```
import { BrowserModule } from '@angular/platform-browser';
import { NgModule } from '@angular/core';
import { AppComponent } from './app.component';
import { NgxFirebaseCms } from 'ngx-firebase-cms';
import { environment } from '../environments/environment';

@NgModule({
  imports: [
    BrowserModule,
    NgxFirebaseCms.forRoot(environment.ngxFirebaseCms)
  ],
  declarations: [ AppComponent ],
  bootstrap: [ AppComponent ]
})
export class AppModule {}
```

### 5. Run your app
```
ng serve
```
Run the serve command and navigate to localhost:4200 in your browser.

### 6. Next step
Next Step: [Documents](#)

## Usage
- coming soon

## Development
- coming soon

## Road Map
- coming soon

## Contributing
- coming soon

## Users
- coming soon

## License
- GNU GPLv3
