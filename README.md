# Webcomponents-update-reminder

An element to remind developers if your element have an update.

(this element won't cause any network request unless the page is loaded from a web server running on `localhost` or a Cloud IDE)

## Notice
You can try the new ES6 version of this element by importing `Webcomponents-update-reminder-es6.html`, which have a lot of new cool stuffs.

## Requirements

* Use Bower & Github to manage your element.

## Get start

To use this element in your components:

```html
<!-- add this to anywhere of your element's template -->
<webcomponents-update-reminder
    repo="PolymerElements/paper-toolbar">
</webcomponents-update-reminder>
```

That's all! When your component have a new version, the user will recieve a info like this:

![a info in console](https://raw.githubusercontent.com/markhuang1212/webcomponents-update-reminder/master/info.JPG)

When the page is loaded from a web server running on `localhost` or a Cloud IDE, the element will read the `version` in your repo master branch's `bower.json` and compare it with the local `bower.json` to detect if there is a new version, **only minor and major version update will remind user to update, unless your element's major version is `0`.**

You need to mention that the `version` tag in your `bower.json` should be look like `X.Y.Z`. We recommend naming tags that fit within [semantic versioning](http://semver.org/).

## API Docs
http://open-elements.org/elements/webcomponents-update-reminder
