### grunt-contrib-watch to the rescue!

    $ npm install grunt-contrib-watch --save-dev

Add the following to your Gruntfile:

    // Watch config
    watch: {
      options: {
        livereload: true
      },
      jshint: { 
        files: '<%= jshint.build.src %>',
        tasks: ['jshint']
      },
      uglify: {
        files: '<%= uglify.build.src %>',
        tasks: ['uglify']
      }
    }

And load the task:

    grunt.loadNpmTasks('grunt-contrib-watch');

note:
<br />
Also make sure that you've got the LiveReload browser plugin installed in your browser of choice.
