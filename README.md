## Gun-ui elements
Gun-Ui is a set of webcomponents that enables you - the frontend developer - to build complex - Gun - applications without writing any ( well...almost) javascript

Every gun-ui- element has just 2 required attributes "soul" and "prop" that will link the element to a certain data-point.

## Purpose
* main element for all 'gun-ui-' elements.
* Setup Gun ( and - optional - `gun-tag`) by just providing attributes
* makes sure that every gun-ui- element has the required properties and methods.
* Creates global nameSpace 'GunUi' where 'GunUi.gun' will be the global Gun instance
* ...and then some...we'll get to that when using the elements

#### Without `gun-ui` none of the gun-ui elements will work!

#### You should use this only once in your main document!

## But Why?
If you don'tunderstand the purpose of Gun-Ui take a look at some of the actual gun-ui- elements. ( Not yet there though :) )

## (NPM) Install Gun and gun-tag
'Gun' is not provided as bower modules so we'll have to use NPM.
```
npm install gun
```
If you want to enable tagging you will have to install `gun-tag` also.
```
npm install gun-tag
```
## (Bower) Install gun-ui
```
bower install gun-ui --save
```
## Your main document
```
<!doctype html>
<html lang="en">
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, minimum-scale=1, initial-scale=1, user-scalable=yes">
    <title>todo</title>
    <meta name="description" content="description">
    <script src="/bower_components/webcomponentsjs/webcomponents-loader.js"></script>

    <!-- import gun-ui -->
    <link rel="import" href="/bower_components/gun-ui/gun-ui.html">
  </head>
  <body>
    <--
      Place gun-ui in your body
      set peers (JSON!)
      set attribute 'use-tags' if you want to enable tagging
    -->
    <gun-ui peers='["http://my-Gun-Server/gun"]' use-tags></gun-ui>
  </body>
</html>
```
That's it, you now have Gun with tagging enabled.

<b>NOTE:<br>
Gun is available as 'GunUi.gun'</b>

## Now what?
Now you are ready to start building great apps with Gun but without having to write javascript :)
