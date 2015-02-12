# Let's create a Computer Services site, describing what we do!

### Let's start with a basic template and build up.

* Create a new directory to work in
* Create a new file called index.html

```
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>Computer Services (demo)</title>
  </head>
  <body>
    <h1>Hello, world! We are computer services!</h1>
  </body>
</html>
```

* Let's initialize a git repository, and, and commit our new file!


### Now let's add Bootstrap to beautify a bit

* [Bootstrap](http://getbootstrap.com/getting-started/) is the most popular HTML, CSS, and JS framework for developing responsive, mobile first projects on the web.
* To use it, we link to the bootstrap css stylesheets 

```
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>Computer Services (demo)</title>
	<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.2/css/bootstrap.min.css">
	<link rel="stylesheet" href="http://getbootstrap.com/examples/justified-nav/justified-nav.css">

  </head>
  <body>
    <h1>Hello, world! We are computer services!</h1>
  </body>
</html>
```

### Build out the navigation

```
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>Computer Services (demo)</title>
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.2/css/bootstrap.min.css">
    <link rel="stylesheet" href="http://getbootstrap.com/examples/justified-nav/justified-nav.css">
  </head>
  <body>
    <div class="container">
      <div class="masthead">
        <nav>
          <ul class="nav nav-justified">
            <li class="active"><a href="#">Home</a></li>
            <li><a href="#">Projects</a></li>
            <li><a href="#">Services</a></li>
            <li><a href="#">Downloads</a></li>
            <li><a href="#">About</a></li>
            <li><a href="#">Contact</a></li>
          </ul>
        </nav>
      </div>
      <h1>Hello, world! We are computer services!</h1>
    </div>
  </body>
</html>
```

* Add, commit changes to git

### Fill in the content sections

```
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>Computer Services (demo)</title>
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.2/css/bootstrap.min.css">
    <link rel="stylesheet" href="http://getbootstrap.com/examples/justified-nav/justified-nav.css">
  </head>
  <body>
    <div class="container">
      <div class="masthead">
        <nav>
          <ul class="nav nav-justified">
            <li class="active"><a href="#">Home</a></li>
            <li><a href="#">Projects</a></li>
            <li><a href="#">Services</a></li>
            <li><a href="#">Downloads</a></li>
            <li><a href="#">About</a></li>
            <li><a href="#">Contact</a></li>
          </ul>
        </nav>
      </div>

      <div class="jumbotron">
        <h1>Hello, world! We are computer services!</h1>
        <p class="lead">Cras justo odio, dapibus ac facilisis in, egestas eget quam. Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa justo sit amet.</p>
        <p><a class="btn btn-lg btn-success" href="#" role="button">Get started today</a></p>
      </div>

      <!-- Example row of columns -->
      <div class="row">
        <div class="col-lg-4">
          <p>Donec id elit non mi porta gravida at eget metus. Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa justo sit amet risus. Etiam porta sem malesuada magna mollis euismod. Donec sed odio dui. </p>
          <p><a class="btn btn-primary" href="#" role="button">View details &raquo;</a></p>
        </div>
        <div class="col-lg-4">
          <h2>Heading</h2>
          <p>Donec id elit non mi porta gravida at eget metus. Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa justo sit amet risus. Etiam porta sem malesuada magna mollis euismod. Donec sed odio dui. </p>
          <p><a class="btn btn-primary" href="#" role="button">View details &raquo;</a></p>
       </div>
        <div class="col-lg-4">
          <h2>Heading</h2>
          <p>Donec sed odio dui. Cras justo odio, dapibus ac facilisis in, egestas eget quam. Vestibulum id ligula porta felis euismod semper. Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa.</p>
          <p><a class="btn btn-primary" href="#" role="button">View details &raquo;</a></p>
        </div>
      </div>

      <!-- Site footer -->
      <footer class="footer">
        <p>&copy; Computer Services 2015</p>
      </footer>
    </div>
  </body>
</html>
```
* Add, commit changes to git

### Let's deploy to github pages!

* Sign in to GitHub
* Create new empty repository
* In git-extensions, point the local repository to the new GitHub [clone url](https://github.com/lfucg/code-reviews/blob/master/static-sites-with-github-pages.md)
* Push your local changes to GitHub
* GitHub should now list your index.html file
* Locally, create a branch called gh-pages off of master
* Push to GitHub
* In a few minutes your project should be deployed at [your-github-username].github.io/[repository-name]
* Take a look at the project on a mobile device. How does it look?

### Helpful links

* http://getbootstrap.com/getting-started/
 