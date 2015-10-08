# Webcomponents-update-reminder
Remind your user to update your components just by adding one line

## About this version

This is the second major update of this element. In this release, I totally redesign the structure of the element. As @ told me the 0.2 version will cause a lot of ajax requests when visiting, the following improvement are made in the 0.3 version:

The main function of this element will only be imported when developing on localhost or an IP address.

By doing this, no Ajax request will be made in production, and the total network requests will under 3k, which can basically be ignored. As it won't import the main function, the performances will be much better than the earlier version. 

Since it won't cause any performances problems in your element, why not use it in your element now?

## Get start
To use this element in your components:
```
<webcomponents-update-reminder
    repo="YOUR ELEMENT'S GITHUB REPO, FOR EXAMPLE: PolymerElements/paper-toolbar">
</webcomponents-update-reminder>
```
That's all! When your component have a new version, the user will recieve a info like this:

![a info in console](https://raw.githubusercontent.com/markhuang1212/webcomponents-update-reminder/master/info.JPG)

The element will read the `version` in your repo master branch's `bower.json` and compare it with the local `bower.json` to detect if there is a new version, **only minor and major version update will remind user to update (unless your element's major version is 0)**

You need to mention that the `version` tag in your `bower.json` should be look like `X.Y.Z`. We recommend naming tags that fit within [semantic versioning](http://semver.org/).

## API Docs
https://markhuang1212.github.io/webcomponents-update-reminder

## Let's build together!
This element is still building. If you're interested in it, you can help building it together!
