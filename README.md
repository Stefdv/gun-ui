## Gun-ui elements
The 'gun-ui' elements are created to use Gun with HTML (Polymer) webcomponents and to allow you to start using the amazing dataViz elements.
## \<gun-ui\>
'gun-ui' is the main component that will load 'Gun' and 'gun-tag' for you. It should be used only once in your main document.

## Install Gun and gun-tag
'Gun' and 'gun-tag' are not provided as bower modules so we'll have to use NPM.

```
npm install gun && npm install gun-tag
```
## Install gun-ui
```
bower install gun-ui --save
```
## Place in your main document
First import 'gun-ui'
```
<head>
  <link rel="import" href="bower_components/gun-ui/gun-ui.html">
</head>
```
Then use it...
```
<body>
  <gun-ui peers='["http://my-Gun-Server/gun"]'></gun-ui>
</body>
```
That's it, you now have Gun with tagging enabled.

<b>NOTE:<br>
Gun will NOT be available in devtools unless you set the attribute 'dev'. Then you will have access to 'devgun'!</b>
```
<gun-ui peers='["http://my-Gun-Server/gun"]' dev></gun-ui>
```
# Now what?
Now you are ready to start using the incredible 'gun-ui-' elements :)
