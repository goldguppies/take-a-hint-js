# take-a-hint-js
Sarcastic linting tool 




######Reporting with Grunt

```npm install grunt-contrib-jshint --save-dev```

Then install our module: (when we get it up on npm)

```npm install take-a-hint```

Finally, set the grunt tasks:

```
grunt.initConfig({
  jshint: {
    beforeconcat: ['src/foo.js', 'src/bar.js'],
    afterconcat: ['dist/output.js'],
    reporter: require('take-a-hint')
  }
});

grunt.loadNpmTasks('grunt-contrib-jshint');```
