<!--
# product-landing-page
FreeCodeCamp Landing Page Challenge


<script src="https://cdn.freecodecamp.org/testable-projects-fcc/v1/bundle.js"></script>
-->

<!DOCTYPE html>
<html>
  <head>
    <meta charset="UTF-8">
    <meta name="website" content="Product Landing Page">
    <title>FreeCodeCamp Product Landing Page</title>

    <style>

    @import 'https://fonts.googleapis.com/css?family=Lato:400,700';

    #body {
      background-color: #eee;
      font-family: 'Lato', sans-serif;
    }

    #page-wrapper {
      position: relative;
    }

    li {
      list-style: none;
    }

    a {
      color: #000;
      text-decoration: none;
    }

    .container {
      max-width: 1000px;
      width: 100%;
      margin: 0 auto;
    }

    .nav-link {}

    i1 {
      font-size: 40px;
      font-weight: 900;
      font-family: Bakery;
    }


    header {
      position: fixed;
      top: 0;
      min-height: 75px;
      padding: 0px 20px;
      display: flex;
      justify-content: space-around;
      align-items: center;
      background-color: #eee;
    }

    @media (max-width: 600px) {
      header {
        flex-wrap: wrap;
      }
    }

    #features {
      margin-top: 30px;
    }


    #features .icon {
      display: flex;
      align-items: center;
      justify-content: center;
      height: 125px;
      width: 20vw;
      color: darkorange;

    }

    @media (max-width: 550px) {
      #features .icon {
        display: none;
      }
    }

    #features .desc {
      display: flex;
      flex-direction: column;
      justify-content: center;
      height: 125px;
      width: 80vw;
      padding: 5px;
    }

    @media (max-width: 550px) {
      #features .desc {
        width: 100%;
        text-align: center;
        padding: 0;
        height: 150px;
      }
    }

    @media (max-width: 650px) {
      #features {
        margin-top: 0;
      }
    }

    #how-it-works {
      margin-top: 50px;
      display: flex;
      justify-content: center;
    }

    #how-it-works > iframe {
      max-width: 560px;
      width: 100%;
    }

    #pricing {
      margin-top: 60px;
      display: flex;
      flex-direction: row;
      justify-content: center;
    }


    .product {
      display: flex;
      flex-direction: column;
      align-items: center;
      text-align: center;
      width: calc(100% / 3);
      margin: 10px;
      border: 1px solid #000;
      border-radius: 3px;
    }

    .product > .level {
      background-color: #ddd;
      color: black;
      padding: 15px 0;
      width: 100%;
      text-transform: uppercase;
      font-weight: 700;
    }

    .product > h2 {
      margin-top: 15px;
    }

    .product > ol {
      margin: 15px 0;
    }

    .product > ol > li {
      padding: 5px 0;
    }

    .product > button {
      border: 0;
      margin: 15px 0;
      background-color: #f1c40f;
      font-weight: 400;
    }

    .product > button:hover {
      background-color: orange;
      transition: background-color 1.5s;
    }

    @media (max-width: 800px) {
      #pricing {
        flex-direction: column;
      }
      .product {
        max-width: 300px;
        width: 100%;
        margin: 0 auto;
        margin-bottom: 10px;

      }
    }


    .logo {
      width: 60vw;
    }

    @media (max-width: 650px) {
      .logo {
        margin-top: 15px;
        width: 100%;
        position: relative;
      }
    }

    .logo > img {
      width: 100%;
      height: 100%;
      max-width: 300px;
      display: flex;
      justify-content: center;
      align-items: center;
      text-align: center;
      margin-left: 20px;
    }

    @media (max-width: 650px) {
      .logo > img {
        margin: 0 auto;
      }
    }

    nav {
      font-weight: 400;
    }

    @media (max-width: 650px) {
      nav {
        margin-top: 10px;
        width: 100%;
        display: flex;
        flex-direction: column;
        align-items: center;
        text-align: center;
        padding: 0 50px;
      }

    nav li {
      padding-bottom: 5px;
      }
    }

    nav > ul {
      width: 35vw;
      display: flex;
      flex-direction: row;
      justify-content: space-around;
    }

    @media (max-width: 650px) {
      nav > ul {
        flex-direction: column;
      }
    }


    #hero {
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      text-align: center;
      height: 200px;
      margin-top: 50px;
    }

    #hero > h2 {
      margin-bottom: 20px;
      word-wrap: break-word;
    }

    #hero input[type='email'] {
      max-width: 275px;
      width: 100%;
      padding: 5px;
    }

    #hero input[type='submit'] {
      max-width: 150px;
      width: 100%;
      height: 30px;
      margin: 15px 0;
      border: 0;
      background-color: #f1c40f;
    }

    #hero input[type='submit']:hover {
      background-color: orange;
      transition: background-color 1s;
    }

    @media (max-width: 650px) {
      #hero {
        margin-top: 120px;
      }
    }

    .btn {
     padding: 0 20px;
     height: 40px;
     font-size: 1em;
     font-weight: 900;
     text-transform: uppercase;
     border: 3px black solid;
     border-radius: 5px;
     background: transparent;
     cursor: pointer;
    }

    .grid {
      display:flex;
    }

    footer {
      margin-top: 30px;
      background-color: #ddd;
      padding: 20px;
    }

    footer > ul {
      display: flex;
      justify-content: flex-end;
    }

    footer > ul > li {
      padding: 0 10px;
    }

    footer > span {
      margin-top: 5px;
      display: flex;
      justify-content: flex-end;
      font-size: 0.9em;
      color: #444;
    }

    </style>

  </head>
  <body id="body">
 <div id="page-wrapper">

   <header id="header">

     <div class="logo">
        <img id="header-img" src="https://s3.amazonaws.com/freecodecamp/original_trombones.png" alt="company logo">
     </div>

     <nav id="nav-bar">
        <ul>
          <li>
            <a class="nav-link" href="#features">Features</a>
          </li>

          <li>
            <a class="nav-link" href="#how-it-works">How It Works</a>
          </li>

          <li>
            <a class="nav-link" href="#pricing">Pricing</a>
          </li>

        </ul>
      </nav>
    </header>

    <div class="container"></div>

    <section id="hero">

      <h2>Handmade Masterpieces</h2>

      <form id="form" action="https://www.freecodecamp.com/email-submit">
        <input id="email" name="email" placeholder="Enter your email address" required type="email"></input>

      <input id="submit" type="submit" value="Get Started" class="btn"></input>
      </form>
    </section>

 <div class="container">

  <section id="features">

    <div class="grid">
      <div class="icon">
        <i1>
        Handmade
        </i1>
      </div>
      <div class="desc">
        <h2>Premium Materials</h2>
        <p>Our instruments are made from the very best, created on-site and prepared to your requirements.</p>
      </div>
    </div>

      <div class="grid">
      <div class="icon">
        <i1>
        Delivery
        </i1>
      </div>
      <div class="desc">
        <h2>Fast Shipping</h2>
        <p>Our instruments are all brought within 24 hours, <i>Guarenteed!</i></p>
      </div>
    </div>

      <div class="grid">
      <div class="icon">
        <i1>
        Quality
        </i1>
      </div>
      <div class="desc">
        <h2>Quality Assurance</h2>
        <p>Our instruments are all tested and assurance of the highest quality is first and foremost.</p>
      </div>
    </div>
  </section>



  <section id="how-it-works">
    <iframe id="video" height="315" src="https://www.youtube-nocookie.com/embed/y8Yv4pnO7qc?rel=0&controls=0&showinfo=0" frameborder="0" allowfullscreen>
    </iframe>
  </section>



  <section id="pricing">
    <div class="product" id="tenor">
      <div class="level">Tenor</div>
      <h2>€600</h2>
      <ol>
        <li>Lorem ipsum.</li>
        <li>Lorem ipsum.</li>
        <li>Lorem ipsum.</li>
      </ol>
      <button class="btn">Select</button>
    </div>

        <div class="product" id="bass">
      <div class="level">Bass Trombone</div>
      <h2>€500</h2>
      <ol>
        <li>Lorem ipsum.</li>
        <li>Lorem ipsum.</li>
        <li>Lorem ipsum.</li>
      </ol>
      <button class="btn">Select</button>
    </div>

        <div class="product" id="sax">
      <div class="level">Saxophone</div>
      <h2>€1200</h2>
      <ol>
        <li>Lorem ipsum.</li>
        <li>Lorem ipsum.</li>
        <li>Lorem ipsum.</li>
      </ol>
      <button class="btn">Select</button>
    </div>
  </section>


  <footer>
 <ul>
   <li>
     <a href="#">Privacy</a>
   </li>
   <li>
     <a href="#">Terms</a>
   </li>
   <li>
     <a href="#">Contract</a>
   </li>
    </ul>
    <span>Copyright 2020, Original Trombones</span>
   </footer>  
 </div>   
  </body>

</html>
