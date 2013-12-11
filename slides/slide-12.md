**grunt-contrib-watch** to the rescue!

    $ npm install grunt-contrib-watch --save-dev

Add the following to your Gruntfile:

		// Watch config
		watch: {
		  options: {
		    livereload: true
		  },
		  js: { 
		    files: ['js/script.js', 'Gruntfile.js'],
		    tasks: ['jshint', 'uglify']
		  }
		}

And load the task:

		  grunt.loadNpmTasks('grunt-contrib-watch');

note:
    Also make sure that you've got the LiveReload browser plugin installed in your browser of choice.
