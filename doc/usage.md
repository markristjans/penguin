
> After downloading penguin, follow these simple steps to get started:

### Customize with Sass

If you choose this way then you should Build Using a Task Runner. penguin uses Grunt for compile our code.

First of all, you should install Node and Grunt.
If you want to build the project locally, you have to run the [Grunt](http://gruntjs.com/) task `grunt build`. This task will concat and minify the sources and create the README.md. Before all this, you do not forget to run `npm install` and `bower install`.


###Compiled and minified CSS and JavaScript.

You should add to project stylesheet and link it in the header of your HTML file, like so:

        <!-- This is how you would link your penguin stylesheet -->
        <link rel="stylesheet" href="dist/css/penguin.min.css">
    </head>

If you are using any penguin JavaScript components, this needs to be loaded on the page. You do not forget add jQuery to project, penguin components require jQuery to be included. We recommend at the end before your closing <body> tags like so:

        <script src="bower_components/jquery/dist/jquery.min.js"></script>
        <script src="dist/js/penguin.min.js"></script>
        <script>
            $('body').modal();
        </script>
    </body>

Also you can load only the components you need for your project:

        <script src="bower_components/jquery/dist/jquery.min.js"></script>
        <!-- Alerts -->
        <script src="dist/js/components/alert.js"></script>
        <!-- Dropdowns -->
        <script src=""dist/js/components/dropdown.js"></script>
        <!-- Modal -->
        <script src=""dist/js/components/modal.js"></script>
        <!-- Spinner -->
        <script src=""dist/js/components/spinner.js"></script>
    </body>