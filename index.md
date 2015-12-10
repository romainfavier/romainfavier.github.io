---
layout: default
title: Titre du site
---

<!DOCTYPE html>
<html lang="en">

<head>

    <meta charset="utf-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <meta name="description" content="">
    <meta name="author" content="">

    <title>Site de Mathilde </title>

    <link href="css/bootstrap.min.css" rel="stylesheet">
    <link href="css/modern-business.css" rel="stylesheet">
    <link href="font-awesome/css/font-awesome.min.css" rel="stylesheet" type="text/css">

</head>

<body>

    <!-- Navigation -->
    <nav class="navbar navbar-inverse navbar-fixed-top" role="navigation">
        <div class="container">
            <!-- Brand and toggle get grouped for better mobile display -->
            <div class="navbar-header">
                <button type="button" class="navbar-toggle" data-toggle="collapse" data-target="#bs-example-navbar-collapse-1">
                    <span class="sr-only">Toggle navigation</span>
                    <span class="icon-bar"></span>
                    <span class="icon-bar"></span>
                    <span class="icon-bar"></span>
                </button>
                <a class="navbar-brand" href="index.html">Start Bootstrap</a>
            </div>
            <!-- Collect the nav links, forms, and other content for toggling -->
            <div class="collapse navbar-collapse" id="bs-example-navbar-collapse-1">
                <ul class="nav navbar-nav navbar-right">
                
                    
                    <li>
                        <a href="contact.html">Contact</a>
                    </li>
		    <li>
                        <a href="billet.html">Billet</a>
                    </li>

                  
                   
                </ul>
            </div> 
            <!-- /.navbar-collapse -->
       </div>
    </nav>
    </br>
<!-- Projects Row -->
		
        <div class="row">
	
		{% for post in site.posts limit:3 %}
			
				
   			
			 		<div class="col-md-4 img-portfolio">
                			<a href="{{ post.url }}">
                    			<img class="img-responsive img-hover" src="http://placehold.it/700x400" alt="">
                			</a>
                			<h3>
                    			<a href="{{ post.url }}">{{ post.title }}</a>
                			</h3>
                			
            				</div>
						
    		{% endfor %}
		
           
           
    

    <!-- jQuery -->
    <script src="js/jquery.js"></script>

    <!-- Bootstrap Core JavaScript -->
    <script src="js/bootstrap.min.js"></script>

    <!-- Script to Activate the Carousel -->
    <script>
    $('.carousel').carousel({
        interval: 5000 //changes the speed
    })
    </script>

</body>

</html>
