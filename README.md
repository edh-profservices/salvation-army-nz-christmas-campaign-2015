# Salvation Army NZ Christmas Campaign 2015

Responsive giving hub for Salvation Army NZ Christmas Campaign 2015.

## Dependencies

- [Node.js](https://nodejs.org/) (v0.10+)
- [Gulp.js](http://gulpjs.com/)

## Set up

1. Clone repository to your local machine:

  ```sh
  git clone https://github.com/everydayhero/salvation-army-nz-christmas-campaign-2015.git
  ```
2. With your terminal/command prompt still open, navigate to your project and install the dependencies (setup may take a few minutes):

  ```sh
  $ cd salvation-army-nz-christmas-campaign-2015
  $ npm run setup
  ```

#### Run Dev

1. Run this command: `npm run start`.
2. Open `http://localhost:3000` in your browser.

At this point you should have a running site visible in your browser. If you skipped the Prismic set up it may be missing content.

## Publish to S3

This task will automatically upload all of your static files (located in `./dist`) to a designated Amazon S3 bucket. Follow the set up:

1. Add a file named `aws.json` to the project root directory. Insert credentials/info based on the following:

  ```json
    {
      "key": "YOUR_AWS_KEY",
      "secret": "YOUR_AWS_SECRET",
      "bucket": "YOUR_BUCKET_NAME",
      "region": "YOUR_BUCKET_REGION"
    }
  ```
2. Run this command `npm run publish`.

**Note:** Keep your AWS key and secret safe! Make sure this file is added to your .gitignore file before pushing your project up to GitHub.


## Commands

```sh
$ npm run setup    # install project dependencies, run an initial build
$ npm run build    # build production assets
$ npm run start    # run a build and start a local server
$ npm run publish  # publish production assets to Amazon S3
```
