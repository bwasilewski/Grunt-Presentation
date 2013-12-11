Update your watch directive:

		// Watch config
		watch: {
		  options: {
		    livereload: true
		  },
		  js: { 
		    files: ['js/script.js', 'Gruntfile.js'],
		    tasks: ['jshint', 'uglify']
		  },
		  sass: {
		    files: ['scss/styles.scss'],
		    tasks: ['sass']
		  }
		}

And load the task:

  	grunt.loadNpmTasks('grunt-contrib-sass');

note:

