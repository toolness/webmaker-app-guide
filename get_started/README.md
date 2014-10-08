# Get started

### Dependencies

To get a local version of Webmaker Mobile running, you'll need to have [git](http://git-scm.com/) and [node](http://nodejs.org/) installed on your local machine.

You'll also need to **globally install [gulp](http://gulpjs.com/)**, which we use for building front-end assets:

```bash
npm install -g gulp
```

*Note: If you get errors globally installing gulp, try `sudo npm install -g gulp`.*

### Clone

In order to contribute to Webmaker Mobile, you'll need to **create your own fork** of Webmaker Mobile and make pull-requests against our master branch.

Clone from your own fork or from the original:

```
git clone https://github.com/mozillafordevelopment/webmaker-app.git
cd mobile-appmaker
```

### Build and develop

To start developing, all you need to do is run the following in the `webmaker-app` directory you just created:

```bash
npm install
gulp dev
```

This will pull down localization files, build the project, start a webserver for you at `http://localhost:8080`, and run a `watch` process so that your front-end assets will be regenerated as you make changes.
