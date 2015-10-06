# Webcomponents-update-reminder
Remind your user to update your components just by adding one line

## Get start
To use this element in your components:
```
<!-- import this element first just like you do to other web components -->
<!-- you can add async tag to this because it won't effect the remder of the page -->
<link rel="import" href="../webcomponents-update-reminder/webcomponents-update-reminder.html" async>

<!-- adding this inside your web component -->
<webcomponents-update-reminder
    src="YOUR ELEMENT'S GITHUB REPO, FOR EXAMPLE: PolymerElements/paper-toolbar">
</webcomponents-update-reminder>
```
That's all! By default, we will read the "version" in bower.json file from element's master branch to detect if there is a new version, only minor and major version update will remind user to update. Your user will recieve a message from console when developing on `localhost` or `127.0.0.1`.

Of course, you can config all of these above yourself by seeing the API Docs below.

## API docs
