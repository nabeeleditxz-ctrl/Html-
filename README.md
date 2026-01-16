<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>TikTok Accounts Marketplace</title>
  <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css">
  <script src="https://identity.netlify.com/v1/netlify-identity-widget.js"></script> <!-- Free Netlify auth -->
</head>
<body>
  <header class="text-center">
    <h1>Sell/Buy TikTok Accounts</h1>
    <button onclick="netlifyIdentity.open()">Login/Sign Up</button> <!-- Auth button -->
  </header>
  <div class="container" id="user-content" style="display:none;"> <!-- Show after login -->
    <h2>Your Dashboard</h2>
    <p>Manage listings here.</p>
  </div>
  <div class="container">
    <div class="row">
      <!-- Listing 1 -->
      <div class="col-md-4">
        <div class="card">
          <img src="account1.jpg" class="card-img-top" alt="Account">
          <div class="card-body">
            <h5>Fashion Account - 15K Followers</h5>
            <p>$75</p>
            <a href="#" class="btn btn-primary">Buy Now</a>
          </div>
        </div>
      </div>
      <div class="col-md-4">
        <div class="card">
          <img src="account1.jpg" class="card-img-top" alt="Account">
          <div class="card-body">
            <h5>Editing Account - 2K Followers - 130k Likes</h5>
            <p>$7</p>
            <a href="#" class="btn btn-primary">Buy Now</a>
          </div>
        </div>
      </div>
      <div class="col-md-4">
        <div class="card">
          <img src="account1.jpg" class="card-img-top" alt="Account">
          <div class="card-body">
            <h5>Fashion Account - 15K Followers</h5>
            <p>$75</p>
            <a href="#" class="btn btn-primary">Buy Now</a>
          </div>
        </div>
      </div>
      <!-- Add more listings -->
    </div>
  </div>
  <footer class="text-center">Disclaimer: Transactions at your own risk.</footer>
  <script>
    netlifyIdentity.on('login', user => { document.getElementById('user-content').style.display = 'block'; });
    netlifyIdentity.on('logout', () => { document.getElementById('user-content').style.display = 'none'; });
  </script>
</body>
</html>
