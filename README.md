
<style>
  /* Page reset */
  body, html {
    margin: 0;
    padding: 0;
    height: 100%;
    overflow: hidden;
    font-family: 'Poppins', sans-serif;
    color: white;
  }

  /* Fullscreen background video */
  video {
    position: fixed;
    top: 0;
    left: 0;
    min-width: 100%;
    min-height: 100%;
    object-fit: cover;
    z-index: -1;
  }

  /* Top heading */
  .page-heading {
    position: absolute;
    top: 20px;
    width: 100%;
    text-align: center;
    font-size: 2.5rem;
    font-weight: bold;
    text-shadow: 0 0 10px rgba(0,0,0,0.6),
                 0 0 20px rgba(255,255,255,0.8);
    animation: glow 2s infinite alternate;
  }

  /* Glow effect */
  @keyframes glow {
    from { text-shadow: 0 0 10px #ff69b4, 0 0 20px #1e90ff; }
    to { text-shadow: 0 0 20px #ff69b4, 0 0 40px #1e90ff; }
  }

  /* Center profile area */
  .center-content {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    text-align: center;
  }

  /* Profile picture */
  .profile {
    width: 260px;
    max-width: 70vw;
    border-radius: 50%;
    border: 8px solid white;
    box-shadow: 
      0 0 30px rgba(255, 105, 180, 0.8),
      0 0 60px rgba(30, 144, 255, 0.6),
      0 8px 25px rgba(0, 0, 0, 0.4);
  }

  /* Clickable name */
  .name-link {
    display: inline-block;
    margin-top: 15px;
    padding: 10px 20px;
    font-size: 1.6rem;
    font-weight: bold;
    color: white;
    background: linear-gradient(90deg, #ff69b4, #1e90ff);
    border-radius: 40px;
    text-decoration: none;
    box-shadow: 0 0 15px rgba(255,255,255,0.5);
    transition: all 0.3s ease-in-out;
  }

  .name-link:hover {
    transform: scale(1.08);
    box-shadow: 0 0 25px rgba(255,255,255,0.8);
  }

  /* Mobile responsive */
  @media (max-width: 600px) {
    .page-heading { font-size: 1.6rem; top: 15px; }
    .name-link { font-size: 1.2rem; padding: 6px 14px; }
  }
</style>
</head>
<body>

<!-- Water background -->
<video autoplay muted loop playsinline>
  <source src="anand.mp4" type="video/mp4">
  Your browser does not support HTML5 video.
</video>

<!-- Top heading -->
<div class="page-heading">WELCOME</div>

<!-- Profile image & name -->
<div class="center-content">
  <img src="image.webp" alt="Anand Shukla" class="profile">
  <br>
  <a href="E.HTML" class="name-link">ANAND SHUKLA</a>
</div>

</body>
</html>
