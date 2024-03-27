# EX01 Developing a Simple Webserver
## Date:

## AIM:
To develop a simple webserver to serve html pages.

## DESIGN STEPS:
### Step 1: 
HTML content creation.

### Step 2:
Design of webserver workflow.

### Step 3:
Implementation using Python code.

### Step 4:
Serving the HTML pages.

### Step 5:
Testing the webserver.

## PROGRAM:
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-QWTKZyjpPEjISv5WaRU9OFeRpok6YctnYmDr5pNlyT2bRjXh0JMhjY6hW+ALEwIH" crossorigin="anonymous">
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.11.3/font/bootstrap-icons.min.css">
</head>
<body>
    
    
    <nav class="navbar navbar-expand-lg bg-body-tertiary">
        
        <div class="container-fluid">
          <a class="navbar-brand" href="#">Navbar</a>
          <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
          </button>
          <div class="collapse navbar-collapse" id="navbarSupportedContent">
            <ul class="navbar-nav me-auto mb-2 mb-lg-0">
              <li class="nav-item">
                <a class="nav-link active" aria-current="page" href="#">Home</a>
              </li>
              <li class="nav-item">
                <a class="nav-link" href="#">Link</a>
              </li>
              <li class="nav-item dropdown">
                <a class="nav-link dropdown-toggle" href="#" role="button" data-bs-toggle="dropdown" aria-expanded="false">
                  Dropdown
                </a>
                <ul class="dropdown-menu">
                  <li><a class="dropdown-item" href="#">Action</a></li>
                  <li><a class="dropdown-item" href="#">Another action</a></li>
                  <li><hr class="dropdown-divider"></li>
                  <li><a class="dropdown-item" href="#">Something else here</a></li>
                </ul>
              </li>
              <li class="nav-item">
                <a class="nav-link disabled" aria-disabled="true">Disabled</a>
              </li>

            </ul>
            
            <div class="input-group mb-3">
                <input type="text" class="form-control" placeholder="Recipient's username" aria-label="Recipient's username" aria-describedby="basic-addon2">
                <span class="input-group-text" id="basic-addon2"><i class="bi bi-search"></i></span>
              </div>
            </form>
          </div>
        </div>
      </nav>
      <div id="carouselExampleDark" class="carousel carousel-dark slide">
        <div class="carousel-indicators">
          <button type="button" data-bs-target="#carouselExampleDark" data-bs-slide-to="0" class="active" aria-current="true" aria-label="Slide 1"></button>
          <button type="button" data-bs-target="#carouselExampleDark" data-bs-slide-to="1" aria-label="Slide 2"></button>
          <button type="button" data-bs-target="#carouselExampleDark" data-bs-slide-to="2" aria-label="Slide 3"></button>
        </div>
        <div class="carousel-inner">
          <div class="carousel-item active" data-bs-interval="10000">
            <img src="2.webp" class="d-block w-100" alt="...">
            <div class="carousel-caption d-none d-md-block">
              <h5 style="color: azure;" >spider man</h5>
              
            </div>
          </div>
          <div class="carousel-item" data-bs-interval="2000">
            <img src="1.jpg" class="d-block w-100" alt="...">
            <div class="carousel-caption d-none d-md-block">
              <h5 style="color: azure;">No way home</h5>
              
            </div>
          </div>
          <div class="carousel-item">
            <img src="3.jpg" class="d-block w-100" alt="...">
            <div class="carousel-caption d-none d-md-block">
              <h5 style="color: azure;">the king of spiders</h5>
              
            </div>
          </div>
        </div>
        <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleDark" data-bs-slide="prev">
          <span class="carousel-control-prev-icon" aria-hidden="true"></span>
          <span class="visually-hidden">Previous</span>
        </button>
        <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleDark" data-bs-slide="next">
          <span class="carousel-control-next-icon" aria-hidden="true"></span>
          <span class="visually-hidden">Next</span>
        </button>
      </div>
      <div style="display: flex;">
      <div class="card" style="width: 18rem; display: flex;">
        <img src="images (1).jpg" class="card-img-top" alt="...">
        <div class="card-body">
          <h5 class="card-title">the power</h5>
          <p class="card-text">
            The sequel arrived two years later and showed Peter at his high school graduation, so he should have been 18 years old</p>
          <a href="https://simple.wikipedia.org/wiki/Spider-Man#:~:text=His%20powers%20were%20super%20strength,to%20that%20of%20a%20spider.&text=S.H.I.E.L.D" class="btn btn-primary">Go somewhere</a>
        </div>
      </div><div class="card" style="width: 18rem;">
        <img src="images (2).jpg" class="card-img-top" alt="...">
        <div class="card-body">
          <h5 class="card-title">Andrew Garfield</h5>
          <p class="card-text">Andrew Garfield Was The Oldest Spider-Man Actor

             The sequel arrived two years later and showed Peter at his high school graduation, so he should have been 18 years old.</p>
          <a href="#" class="btn btn-primary">Go somewhere</a>
        </div>
      </div><div class="card" style="width: 18rem; ">
        <img src="images.jpg" class="card-img-top" alt="...">
        <div class="card-body">
          <h5 class="card-title">wed man</h5>
          <p class="card-text">The sequel arrived two years later and showed Peter at his high school graduation, so he should have been 18 years old.</p>
          <a href="#" class="btn btn-primary">Go somewhere</a>
        </div>
      </div><div class="card" style="width: 18rem; ">
        <img src="download (1).jpg" class="card-img-top" alt="...">
        <div class="card-body">
          <h5 class="card-title">super spider</h5>
          <p class="card-text">The sequel arrived two years later and showed Peter at his high school graduation, so he should have been 18 years old</p>
          <a href="#" class="btn btn-primary">Go somewhere</a>
        </div>
      </div>
    </div>
      <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js" integrity="sha384-YvpcrYf0tY3lHB60NNkmXc5s9fDVZLESaAA55NDzOxhy9GkcIdslK1eN7N6jIeHz" crossorigin="anonymous"></script>
</body>
</html>
```
## OUTPUT:
![alt text](<Screenshot 2024-03-27 081137.png>)

## RESULT:
The program for implementing simple webserver is executed successfully.
