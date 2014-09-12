# Get started

### Dependencies

To get a local version of Mobile Appmaker running, you'll need to have [git](http://git-scm.com/), [node](http://nodejs.org/), and [gulp](http://gulpjs.com/) installed on your local machine.

### Clone

In order to contribute to Mobile Appmaker, you'll need to **create your own fork** of Mobile Appmaker and make pull-requests against our master branch.

Clone from your own fork or from the original:

```
git clone https://github.com/mozillafordevelopment/mobile-appmaker.git
cd mobile-appmaker
```

### Build and develop

To start developing, all you need to do is run the following in the `mobile-appmaker` directory you just created:

```bash
npm install
gulp dev
```

This will pull down localization files, build the project, start a webserver for you at `http://localhost:8080`, and run a `watch` process so that your front-end assets will be regenerated as you make changes.
