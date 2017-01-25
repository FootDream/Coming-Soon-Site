# FootDream Pre-launch Site

To run the site locally

1. Clone this repo
1. `cd` into the cloned directory
1. Run `bower install`
1. Run `npm install`
1. Run `gulp serve`
1. The site should be live at localhost:9000

> If you don't have gulp or bower, you may install it with `npm install -g gulp bower`

To create a dist build, run `gulp build`

# Deploy

The site is hosted on GitHub pages. You need to have access to the target repo for the deployment to work

1. Run `git add origin github git@github.com:FootDream/footdream.github.io.git`
1. Build the site using `gulp build`
1. Publish to Github Pages using `gulp deploy`

You might see the following error

```bash
Error: Command failed: /bin/sh -c git push --set-upstream github master
fatal: 'github' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.

    at ChildProcess.exithandler (child_process.js:213:12)
    at emitTwo (events.js:87:13)
    at ChildProcess.emit (events.js:172:7)
    at maybeClose (internal/child_process.js:827:16)
    at Process.ChildProcess._handle.onexit (internal/child_process.js:211:5)
```

In that case `cd` into the `.publish` directory and push to `origin` to deploy.
