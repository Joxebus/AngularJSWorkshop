# Setup AngularJS Application

The following steps are to setup the first AngularJS application.

- Download AngularJS from the site https://angularjs.org/
- Create `index.html` file
- Add `angular.js` script in the head tag
- Add `ng-app` directive to on the `<html>` tag like this `<html ng-app>`

By doing that we are declaring this is an **AngularJS** application.

## Using directives

### ng-if
Add a paragraph with conditional directive `ng-if`

```
<p ng-if="true">Good morning</p>
```

This will be true always until we change it to false

```
<p ng-if="false">Good morning</p>
```

Now that is set to false the paragraph will not be shown.

### ng-init

Add a directive `ng-init` to initialize values to be used on the `ng-if`

```html
<body ng-init="hourOfDay = 14">
    <h1>Hello Angular!</h1>
    <p ng-if="hourOfDay < 12">Good morning</p>
    <p ng-if="hourOfDay > 11 && hourOfDay < 18 ">Good afternoon</p>
    <p ng-if="hourOfDay > 17">Good evening</p>
</body>
```