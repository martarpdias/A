#projeto

<div?php
session_start();
if (!isset($_SESSION['user_id'])) {
  header("Location: ../register.html");
  exit();
}
?>

<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Artificial Inteligence Conference 2024</title>
  <link rel="stylesheet" href="homepage.css" />

  <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.6.0/jquery.min.js"></script>
  <script src="https://cdnjs.cloudflare.com/ajax/libs/jquery.cycle2/2.1.6/jquery.cycle2.min.js"></script>
  <style>
   
    .register-presence-link {
      text-align: center;
      margin-top: 20px;
      font-size: 18px;
      color: white;
      background-color: rgb(74, 74, 231);
      padding: 10px 20px;
      border-radius: 5px;
      transition: background-color 0.3s ease;
      margin-left: 5%;
      width: 50%;
        
    }

    .register-presence-link:hover {
      background-color: white;
      color: rgb(74, 74, 231);
      border: 2px solid rgb(74, 74, 231) ;
    }

    @media screen and (max-width: 768px) {
      .slider-wrapper {
        width: fit-content;
        height: fit-content;
      }
    }
    </style>
</head>

<body>
  <header>
    <div class="container">
      <div id="branding">
        <h1><span class="highlight">A</span>rtificial <span class="highlight">I</span>nteligence Conference <span class="highlight">2024</span></h1>
      </div>
      <nav>
        <ul>
          <li class="current"><a href="homepage.php">Home</a></li>
          <li><a href="tracks.php"> Tracks</a></li>
          <li><a href="sessions.php">Program - Sessions</a></li>
          <li><a href="Article_table.html" >Articles</a></li>
          <li><a href="location.php">Location</a></li>
          <li><a href="otherinfo.php">Other Informations</a></li>
          <li>
            <a href="profile.php">
          <li style="margin-top: -7px">
            <img src="./images/profile.jpg" alt="profile" width="40px" />
          </li></a>
          </li>
        </ul>
      </nav>
    </div>
  </header>
  <class="container" style="margin: auto">
  <h1>Welcome to the Artificial Inteligence Conference 2024!</h1>
    <div class="text" style="margin-top: 30px">
      <hr>
      <h3>
        About this Conference
      </h3>
      <p>
        Welcome to the AI Conference 2024, the premier event for professionals, enthusiasts, and innovators in the field of artificial intelligence. Join us as we explore the latest advancements, groundbreaking research, and real-world applications of AI technology. This conference is an unparalleled opportunity to connect with leading experts, network with like-minded individuals, and gain insights into the future of AI.
      </p>
      <p>Our program features keynote speeches from industry pioneers, hands-on workshops, panel discussions, and much more. Whether you're a seasoned professional or just starting your journey in AI, this conference offers something for everyone. Don't miss this chance to be part of a transformative experience that will inspire and equip you to make impactful contributions to the AI landscape.
      </p>
      <hr>
      <br>
    </div>
    </h1>
  
    <h3 style="display: flex; justify-content: center"></h3>
    <a href="presence_form.php" class="register-presence-link">Register Here </a>
    <br>
    <br>
    <br>
    <br>
  </div>


  <footer>
  AI Conference Â© 2024
  </footer>
  </body>

<script>
  $(document).ready(function () {
    var slider = $(".slider").cycle({
      fx: "scrollHorz",
      speed: 1000,
      timeout: 3000,
    });

    $("#next").click(function () {
      slider.cycle("next");
    });

    $("#prev").click(function () {
      slider.cycle("prev");
    });
  });
</script>

</html>