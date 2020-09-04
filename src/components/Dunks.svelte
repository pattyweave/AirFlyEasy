<script>

</script>

<style>
  section {
    background-color: black;
    height: 85vh;
    width: 100%;
    color: white;
    border-bottom: 2px dashed #922cf8;
  }

  h1 {
    font-size: 5rem;
    font-weight: 900;
  }

  video {
    border: 10px solid darkgray;
  }

  .portrait {
    width: 300px;
    border-radius: 10px;
  }

  .landscape {
    width: 500px;
    border-radius: 10px;
  }

  @media screen and (min-width: 20rem) {
    .left,
    .right,
    .left2,
    .right2 {
      width: 100%;
      text-align: center;
      padding-top: 20px;
    }
  }

  @media screen and (min-width: 70rem) {
    .left {
      float: left;
      width: 30%;
      text-align: center;
      padding-top: 50px;
    }
    .right {
      float: right;
      width: 70%;
      text-align: center;
      padding-top: 150px;
    }
    .left2 {
      float: left;
      width: 50%;
      text-align: center;
      padding-top: 75px;
    }
    .right2 {
      float: right;
      width: 50%;
      text-align: center;
      padding-top: 50px;
    }
  }
</style>

<section>
  <div class="left">
    <video autoplay loop muted class="portrait">
      <source src="dunk.mp4" type="video/mp4" />
    </video>
  </div>
  <div class="right">
    <h1>Dunk Harder.</h1>
    <h2>
      Air Fly Easy gives you the tools to take your vertical to the next level.
      Get a leg up on the competition by signing up today.
    </h2>
  </div>
</section>

<section>
  <div class="left2">
    <h1>More Bounce.</h1>
    <h2>
      After just 6 weeks of workouts you'll feel more bounce in your jump and
      more spring in every step. Air Fly Easy rewires your muscles to be quicker
      and stronger.
    </h2>
  </div>
  <div class="right2">
    <video autoplay loop muted class="landscape">
      <source src="landscape.mp4" type="video/mp4" />
    </video>
  </div>
</section>

<section>
  <div  class="left">
    <video autoplay loop muted class="portrait">
      <source src="hurdles.mp4" type="video/mp4" />
    </video>
  </div>
  <div class="right">
    <h1>Workout Anywhere.</h1>
    <h2>
      No need for a gym or weight room to get better. Work out at home, in your yard, or at the park. All of the 
      Air Fly Easy workouts are designed to be able to be done anywhere.
    </h2>
  </div>
</section>
