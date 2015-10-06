# Webcomponents-update-reminder
Remind your user to update your components just by adding one line

## Get start
To use this element in your components:
```
<!-- import this element just like you do to other web components -->
<!-- you can add async tag to this as it won't effect the render of the page -->
<link rel="import" href="../webcomponents-update-reminder/webcomponents-update-reminder.html" async>

<!-- adding this inside your web component -->
<webcomponents-update-reminder
    src="YOUR ELEMENT'S GITHUB REPO, FOR EXAMPLE: PolymerElements/paper-toolbar">
</webcomponents-update-reminder>
```
That's all! When your component have a new version, the user will recieve a info like this:

![a info in console](https://raw.githubusercontent.com/markhuang1212/webcomponents-update-reminder/master/info.JPG)


By default, we will read the "version" in `bower.json` file from element's master branch to and compare it with the local `bower.json` detect if there is a new version, only minor and major version update will remind user to update (unless your element's major version is 0). Your user will recieve a message from console when developing on `localhost` or `127.0.0.1`.

You need to mention that the `version` tag in your `bower.json` should be look like `X.Y.Z` and fit within [semantic versioning](http://semver.org/).

## Contributing

Webcomponents-update-reminder is a new project. Your bug reports, PRs for improvements, docs and anything you think would improve this element are welcomed.
