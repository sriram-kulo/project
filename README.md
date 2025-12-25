# Project Responsive Web Design using Bootstrap
# Date:
# AIM:
To create a simplified clone of Dribbble (https://dribbble.com/) landing page.

# DESIGN STEPS:
## Step 1:
Clone the repository from GitHub.

## Step 2:
Create Django Admin project.

## Step 3:
Create a New App under the Django Admin project.

## Step 4:
Insert the necessary CSS and JavaScript files as external in order to use Bootstrap.

## Step 5:
Create a HTML file and include the needed Bootstrap components.

## Step 6:
Publish the website in the LocalHost.

# PROGRAM :
```
home.html

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <!-- ✅ Bootstrap CSS CDN -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">

  <title>Dribble</title>
  <style>
    .sort-wrapper {
    width: 100%;
    text-align: right;
    margin-bottom: 20px;
    font-family: 'CosmicSerif', serif;
}

#sortSelect {
    padding: 5px 10px;
    font-size: 16px;
    border-radius: 10px;
    border: 1px solid #ddd;
    font-family: 'CosmicSerif', serif;
    background-color: white;
}
#sortSelect option:checked {
    background: #d9d9d9; /* highlight color */
    color: #000;
}
.slider {
  position: relative;
  width: 100%;
  overflow: hidden;
}

.slides {
  display: flex;
  width: 100%;
}
    </style>
</head>
<body>
    <nav class="navbar navbar-expand-lg bg-body-tertiary">
  <div class="container-fluid">
    <a class="navbar-brand" href="#">Dribbble</a>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarSupportedContent">
      <ul class="navbar-nav me-auto mb-2 mb-lg-0">
        <li class="nav-item">
          <a class="nav-link active" aria-current="page" href="home.html">Home</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="about.html">About</a>
        </li>
        <li class="nav-item dropdown">
          <a class="nav-link dropdown-toggle" href="#" role="button" data-bs-toggle="dropdown" aria-expanded="false">
            Explore
          </a>
          <ul class="dropdown-menu">
            <li><a class="dropdown-item" href="product.html">Popular</a></li>
            <li><hr class="dropdown-divider"></li>
            <li><a class="dropdown-item" href="product.html">Product design</a></li>
            <li><a class="dropdown-item" href="product.html">Animation</a></li>
            
            <li><a class="dropdown-item" href="product.html">Web design</a></li>
            <li><a class="dropdown-item" href="product.html">Illustration</a></li>
          </ul>
        </li>
        <li class="nav-item">
          <a class="nav-link disabled" aria-disabled="true">Preminum</a>
        </li>
      </ul>
      <form class="d-flex" role="search">
        <input class="form-control me-2" type="search" placeholder="Search" aria-label="Search"/>
        <button class="btn btn-outline-success" type="submit">Search</button>
      </form>
    </div>
  </div>
</nav>
<section class="slider">
  <div class="slides">
    <img src="sli.png" class="slide">
  </div>
</section>
 <div class="container mt-4">
        <div class="text-center mb-4 header-section">
            <h2>What are you working on?</h2>
            <p class="lead"><h2>Dribbble is show and tell for designers.</h2></p>
        </div>
<section class="grid-section">
    <h2 class="grid-title">Our products</h2>
<div class="sort-wrapper">
    <select id="sortSelect">
        <option value="default">Sort By</option>
        <option value="priceLow">Price: Low → High</option>
        <option value="priceHigh">Price: High → Low</option>
        <option value="nameAZ">Name: A → Z</option>
        <option value="nameZA">Name: Z → A</option>
    </select>
</div>
   

        <div class="row gallery-section">
            
            <div class="col-md-3 col-sm-6 mb-4">
                <div class="card shadow gallery-item">
                    <img src="w1.png" class="card-img-top gallery-img">
                    <div class="card-body text-center">
                        <p class="card-title">Web design</p>
                        <small class="text-muted">Permadi Satria Dewanto</small>
                    </div>
                </div>
            </div>
            <div class="col-md-3 col-sm-6 mb-4">
                <div class="card shadow gallery-item">
                    <img src="w2.png" class="card-img-top gallery-img">
                    <div class="card-body text-center">
                        <p class="card-title">Web design</p>
                        <small class="text-muted">Zikospace</small>
                    </div>
                </div>
            </div>
            <div class="col-md-3 col-sm-6 mb-4">
                <div class="card shadow gallery-item">
                    <img src="i1.png" class="card-img-top gallery-img">
                    <div class="card-body text-center">
                        <p class="card-title">Illustration</p>
                        <small class="text-muted">Taras Migulko for Emote</small>
                    </div>
                </div>
            </div>
            <div class="col-md-3 col-sm-6 mb-4">
                <div class="card shadow gallery-item">
                    <img src="i2.png" class="card-img-top gallery-img">
                    <div class="card-body text-center">
                        <p class="card-title">Illustration</p>
                        <small class="text-muted">GyGinfographics</small>
                    </div>
                </div>
            </div>
            
            <div class="col-md-3 col-sm-6 mb-4">
                <div class="card shadow gallery-item">
                    <img src="p1.png" class="card-img-top gallery-img">
                    <div class="card-body text-center">
                        <p class="card-title">Product design</p>
                        <small class="text-muted">Madhu Miah</small>
                    </div>
                </div>
            </div>
            <div class="col-md-3 col-sm-6 mb-4">
                <div class="card shadow gallery-item">
                    <img src="a1.png" class="card-img-top gallery-img">
                    <div class="card-body text-center">
                        <p class="card-title">Animation</p>
                        <small class="text-muted">Esli Becerra</small>
                    </div>
                </div>
            </div>
            <div class="col-md-3 col-sm-6 mb-4">
                <div class="card shadow gallery-item">
                    <img src="w3.png" class="card-img-top gallery-img">
                    <div class="card-body text-center">
                        <p class="card-title">Web design</p>
                        <small class="text-muted">Musemind Branding & Web Design for Musemind</small>
                    </div>
                </div>
            </div>
            <div class="col-md-3 col-sm-6 mb-4">
                <div class="card shadow gallery-item">
                    <img src="a2.png" class="card-img-top gallery-img">
                    <div class="card-body text-center">
                        <p class="card-title">Animation</p>
                        <small class="text-muted">Esli Becerra</small>
                    </div>
                </div>
            </div>
        </div>
    </div>
</section>
    
        <footer class="bg-dark text-white text-center py-3">
        <p><h2>© Dribbble. All rights reserved.</h2></p>
    </footer>

  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>


about.html

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <!-- ✅ Bootstrap CSS CDN -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">

  <title>Dribble</title>
  <style>
    .sort-wrapper {
    width: 100%;
    text-align: right;
    margin-bottom: 20px;
    font-family: 'CosmicSerif', serif;
}

#sortSelect {
    padding: 5px 10px;
    font-size: 16px;
    border-radius: 10px;
    border: 1px solid #ddd;
    font-family: 'CosmicSerif', serif;
    background-color: white;
}
#sortSelect option:checked {
    background: #d9d9d9; /* highlight color */
    color: #000;
}
.slider {
  position: relative;
  width: 100%;
  overflow: hidden;
}

.slides {
  display: flex;
  width: 100%;
}
    </style>
</head>
<body>
    <nav class="navbar navbar-expand-lg bg-body-tertiary">
  <div class="container-fluid">
    <a class="navbar-brand" href="#">Dribbble</a>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarSupportedContent">
      <ul class="navbar-nav me-auto mb-2 mb-lg-0">
        <li class="nav-item">
          <a class="nav-link active" aria-current="page" href="home.html">Home</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="about.html">About</a>
        </li>
        <li class="nav-item dropdown">
          <a class="nav-link dropdown-toggle" href="#" role="button" data-bs-toggle="dropdown" aria-expanded="false">
            Explore
          </a>
          <ul class="dropdown-menu">
            <li><a class="dropdown-item" href="product.html">Popular</a></li>
            <li><hr class="dropdown-divider"></li>
            <li><a class="dropdown-item" href="product.html">Product design</a></li>
            <li><a class="dropdown-item" href="product.html">Animation</a></li>
            
            <li><a class="dropdown-item" href="product.html">Web design</a></li>
            <li><a class="dropdown-item" href="product.html">Illustration</a></li>
          </ul>
        </li>
        <li class="nav-item">
          <a class="nav-link disabled" aria-disabled="true">Disabled</a>
        </li>
      </ul>
      <form class="d-flex" role="search">
        <input class="form-control me-2" type="search" placeholder="Search" aria-label="Search"/>
        <button class="btn btn-outline-success" type="submit">Search</button>
      </form>
    </div>
  </div>
</nav>

<div class="container text-center">
  <div class="row">
    <div class="col">
      <h1>About Dribbble</h1>
    </div>
  </div>
  <div class="row">
    <div class="col">
      <p>Dribbble began in 2009 as a small, invite-only space for designers to share work and feedback. It quickly became known as the design world’s “cool kids’ table,” where creativity, community, and craft came together.

In 2021, we opened our doors to all designers. Dropping the invite-only model brought in fresh talent while keeping the trusted vibe that made Dribbble special.

Then in 2024, we launched the Dribbble Marketplace. It was a game-changer. Designers could now sell work, land clients, and grow their income, all in one place.

Now, we’re focused on helping designers do work they’re proud of and get paid for it. We’ve shifted from ad-based to revenue-sharing, putting our mission at the core: helping creatives thrive creatively and financially. Supporting creativity isn’t just our motto. It’s the future we’re building together.</p>
    </div>
  </div>
  <div class="row">
    <div class="col">
      <h1>We provide</h1>
    </div>
  </div>
    <div class="row">
        <div class="col">
            <p>A platform to showcase your design work.</p>
            <p>Opportunities to connect with potential clients and collaborators.</p>
            <p>Resources and inspiration from a vibrant design community.</p>
            <p>Tools to help you grow your freelance business.</p>
        </div>
        <div class="row">
    <div class="col">
      <h1>Contact</h1>
    </div>
  </div>
    <div class="row">
        <div class="col">
            <p>email:dribble@gmail.com</p>
            <p>phone: +62 81234567890</p>
            <p>address: Jl. Merdeka No.123, Jakarta, Indonesia</p>
            <p>social media: @dribble</p>
        </div>
</div>
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>


product.html<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <!-- ✅ Bootstrap CSS CDN -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">

  <title>Dribble</title>
  <style>
    .sort-wrapper {
    width: 100%;
    text-align: right;
    margin-bottom: 20px;
    font-family: 'CosmicSerif', serif;
}

#sortSelect {
    padding: 5px 10px;
    font-size: 16px;
    border-radius: 10px;
    border: 1px solid #ddd;
    font-family: 'CosmicSerif', serif;
    background-color: white;
}
#sortSelect option:checked {
    background: #d9d9d9; /* highlight color */
    color: #000;
}
.slider {
  position: relative;
  width: 100%;
  overflow: hidden;
}

.slides {
  display: flex;
  width: 100%;
}
    </style>
</head>
<body>
    <nav class="navbar navbar-expand-lg bg-body-tertiary">
  <div class="container-fluid">
    <a class="navbar-brand" href="#">Dribbble</a>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarSupportedContent">
      <ul class="navbar-nav me-auto mb-2 mb-lg-0">
        <li class="nav-item">
          <a class="nav-link active" aria-current="page" href="home.html">Home</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="about.html">About</a>
        </li>
        <li class="nav-item dropdown">
          <a class="nav-link dropdown-toggle" href="#" role="button" data-bs-toggle="dropdown" aria-expanded="false">
            Explore
          </a>
          <ul class="dropdown-menu">
            <li><a class="dropdown-item" href="product.html">Popular</a></li>
            <li><hr class="dropdown-divider"></li>
            <li><a class="dropdown-item" href="product.html">Product design</a></li>
            <li><a class="dropdown-item" href="product.html">Animation</a></li>
            
            <li><a class="dropdown-item" href="product.html">Web design</a></li>
            <li><a class="dropdown-item" href="product.html">Illustration</a></li>
          </ul>
        </li>
        <li class="nav-item">
          <a class="nav-link disabled" aria-disabled="true">Disabled</a>
        </li>
      </ul>
      <form class="d-flex" role="search">
        <input class="form-control me-2" type="search" placeholder="Search" aria-label="Search"/>
        <button class="btn btn-outline-success" type="submit">Search</button>
      </form>
    </div>
  </div>
</nav>

<section class="grid-section">
    <h2 class="grid-title">Our products</h2>
<div class="sort-wrapper">
    <select id="sortSelect">
        <option value="default">Sort By</option>
        <option value="priceLow">Price: Low → High</option>
        <option value="priceHigh">Price: High → Low</option>
        <option value="nameAZ">Name: A → Z</option>
        <option value="nameZA">Name: Z → A</option>
    </select>
</div>
   

        <div class="row gallery-section">
            
            <div class="col-md-3 col-sm-6 mb-4">
                <div class="card shadow gallery-item">
                    <img src="w1.png" class="card-img-top gallery-img">
                    <div class="card-body text-center">
                        <p class="card-title">Web design</p>
                        <small class="text-muted">Permadi Satria Dewanto</small>
                    </div>
                </div>
            </div>
            <div class="col-md-3 col-sm-6 mb-4">
                <div class="card shadow gallery-item">
                    <img src="w2.png" class="card-img-top gallery-img">
                    <div class="card-body text-center">
                        <p class="card-title">Web design</p>
                        <small class="text-muted">Zikospace</small>
                    </div>
                </div>
            </div>
            <div class="col-md-3 col-sm-6 mb-4">
                <div class="card shadow gallery-item">
                    <img src="i1.png" class="card-img-top gallery-img">
                    <div class="card-body text-center">
                        <p class="card-title">Illustration</p>
                        <small class="text-muted">Taras Migulko for Emote</small>
                    </div>
                </div>
            </div>
            <div class="col-md-3 col-sm-6 mb-4">
                <div class="card shadow gallery-item">
                    <img src="i2.png" class="card-img-top gallery-img">
                    <div class="card-body text-center">
                        <p class="card-title">Illustration</p>
                        <small class="text-muted">GyGinfographics</small>
                    </div>
                </div>
            </div>
            
            <div class="col-md-3 col-sm-6 mb-4">
                <div class="card shadow gallery-item">
                    <img src="p1.png" class="card-img-top gallery-img">
                    <div class="card-body text-center">
                        <p class="card-title">Product design</p>
                        <small class="text-muted">Madhu Miah</small>
                    </div>
                </div>
            </div>
            <div class="col-md-3 col-sm-6 mb-4">
                <div class="card shadow gallery-item">
                    <img src="a1.png" class="card-img-top gallery-img">
                    <div class="card-body text-center">
                        <p class="card-title">Animation</p>
                        <small class="text-muted">Esli Becerra</small>
                    </div>
                </div>
            </div>
            <div class="col-md-3 col-sm-6 mb-4">
                <div class="card shadow gallery-item">
                    <img src="w3.png" class="card-img-top gallery-img">
                    <div class="card-body text-center">
                        <p class="card-title">Web design</p>
                        <small class="text-muted">Musemind Branding & Web Design for Musemind</small>
                    </div>
                </div>
            </div>
            <div class="col-md-3 col-sm-6 mb-4">
                <div class="card shadow gallery-item">
                    <img src="a2.png" class="card-img-top gallery-img">
                    <div class="card-body text-center">
                        <p class="card-title">Animation</p>
                        <small class="text-muted">Esli Becerra</small>
                    </div>
                </div>
            </div>
        </div>
    </div>
</section>
    
        <footer class="bg-dark text-white text-center py-3">
        <p><h2>© Dribbble. All rights reserved.</h2></p>
    </footer>

  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>

```
# OUTPUT:
<img width="1900" height="966" alt="529067022-94052188-f303-48cd-9445-3a940b1789ae" src="https://github.com/user-attachments/assets/3910e255-6569-41ed-9c66-6869321024b4" />
<img width="1896" height="964" alt="529066982-41f77028-52b4-4ca9-9a98-7e875ada8bb0" src="https://github.com/user-attachments/assets/efc24bb8-12eb-4487-9072-92a7f51e3c45" />
<img width="1919" height="970" alt="529067071-449d02a0-cea6-47cc-a53c-9c9e575d6ecf" src="https://github.com/user-attachments/assets/f539ee5b-2e07-4e11-895b-5b38f50ad7a6" />
<img width="1900" height="950" alt="529067117-c4255257-591a-4e8c-ba65-16d0aae9a801" src="https://github.com/user-attachments/assets/f97080e7-f2cd-4e3c-b074-792ce735b2a6" />
<img width="1901" height="950" alt="529067150-3361fcb9-b288-42a4-bd31-44c428588a10" src="https://github.com/user-attachments/assets/1554c314-751e-4beb-bcc0-fccfa2ba3ff8" />

# RESULT:
The Project for responsive web design using Bootstrap is completed successfully.
