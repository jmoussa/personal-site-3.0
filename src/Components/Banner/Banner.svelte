<script>
  export let bannerData = {};
  const { DESCRIPTION, NAME, GREETING, TAGLINE } = bannerData;
</script>

<!------------------------------------------->
<!----------------MARKUP----------------------->
<!------------------------------------------->
<section class="main-bgcolor light-color" id="banner">
  <div class="container">
    <div class="row">
      <div class="col-md-6 valign-center">
        <div class="header">
          <span>
            {GREETING}
            <span class="emphasis">{NAME}</span>
          </span>
          <p>{TAGLINE}</p>
        </div>
        <p class="description">
          {DESCRIPTION}
          <a
            style="color:skyblue;"
            href="https://disney.com"
            target="_blank"
            rel="noopener noreferrer">Disney</a
          >.
        </p>

        <!--<a href={TWITTER_URL} target="_blank" class="light-color">
          {TWITTER_TAGLINE}
        </a> -->
      </div>
      <div class="col-md-6">
        <img src="images/banner.png" alt="" class="img-fluid" />
      </div>
    </div>
  </div>
  <!-- <img src="images/wave1.png" alt="" class="wave-img" /> -->
</section>

<!------------------------------------------->
<!----------------STYLE----------------------->

<!------------------------------------------->
<style>
  section {
    padding-top: 5%;
  }

  h1 {
    font-size: 52px;
    font-weight: 350;
    margin-top: 100px;
    text-transform: uppercase;
  }
  h3 {
    font-size: 24px;
    font-weight: 200;
    /* text-transform: uppercase; */
  }
  .header {
    font-size: x-large;
    width: 100%;
    color: #cdcdcd;
  }
  .description {
    color: #cdcdcd;
  }
  .emphasis {
    font-weight: 400;
    font-size: 3rem;
    color: #fff;
  }

  .img-fluid {
    height: auto;
    margin: 1rem;
  }
  .row {
    padding-bottom: 3rem;
  }

  .col-md-6 {
    display: flex;
    flex-direction: column;
    justify-content: center;
  }
</style>
