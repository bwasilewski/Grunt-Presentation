Update your watch directive:

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
      },
      sass: {
        files: '<%= sass.dist.src %>',
        tasks: ['sass']
      }
		}

And load the task:

  	grunt.loadNpmTasks('grunt-contrib-sass');



