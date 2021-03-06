# NodeJS demo project for Jenkins course

## Setup

- Setup NodeJS Plugin in Jenkins, globally, under ```Jenkins -> Administrar Jenkins -> Global Tool Configuration```. Screenshots for guidance: [here](https://www.dropbox.com/s/ksg8u00gu3x0k9q/Screenshot%202016-09-15%2010.58.38.png?dl=0) and [here](https://www.dropbox.com/s/zr195ttq70uq98e/Screenshot%202016-09-15%2011.06.48.png?dl=0)

- Create a job and configure a job. Don't forget to check this setting for npm to work [this](https://www.dropbox.com/s/pnzflq5w1alxsuk/Screenshot%202016-09-15%2011.25.55.png?dl=0)

- Install the requirements (package.json has them all) and run the tests:

```bash
$ npm install
$ npm test
```

Something like this should be the output of the latest command:

```bash
--> converter (git: master) $ npm test

> converter@0.0.0 test /Users/matiasherranz/DevSantex/Train/JenkinsCI/nodejenkins/converter
> mocha --reporter spec



  Color Code Converter
    RGB to Hex conversion
      ✓ converts the basic colors
    Hex to RGB conversion
      ✓ converts the basic colors


  2 passing (11ms)
  ```
