<script>
  export let socialData = {};
  const { HEADING, DESCRIPTION } = socialData;
</script>
<!------------------------------------------->
<!----------------MARKUP----------------------->
<!------------------------------------------->
<section id="social-media" class="section grey-bgcolor">
  <div class="container text-center">
    <h2 class="title text-center">{HEADING}</h2>
    <div class="social-icons section-body">
        <div class="flex-social-item">
          <a class="linkedin" href="https://linkedin.com/in/jmoussa" rel="noopener noreferrer" target="_blank"><span>LinkedIn</span></a>
          <!-- <span class="social-media-link">LinkedIn</span> -->
        </div>
        <div class="flex-social-item">
          <a class="instagram" href="https://instagram.com/jmoussa.io" rel="noopener noreferrer" target="_blank"><span>Instagram</span></a>
          <!-- <span class="social-media-link">Instagram</span> -->
        </div>
        <div class="flex-social-item">
          <a class="twitter" href="https://twitter.com/j__moussa" rel="noopener noreferrer" target="_blank"><span>Twitter</span></a>
          <!-- <span class="social-media-link">Twitter</span> -->
        </div>
        <div class="flex-social-item">
          <a class="github" href="https://github.com/jmoussa" rel="noopener noreferrer" target="_blank"><span>GitHub</span></a>
          <!-- <span class="social-media-link">Github</span> -->
        </div>
        <div class="flex-social-item">
          <a class="my-resume" href="./resume.pdf" rel="noopener noreferrer" target="_blank"><span>Resume</span></a>
          <!-- <span class="social-media-link">Resume</span> -->
        </div>
    </div>
    <span class="description text-center">{DESCRIPTION}</span>
  </div>
</section>
<!------------------------------------------->
<!----------------STYLE----------------------->
<!------------------------------------------->
<style lang="scss">
.social-icons {
  margin: auto;
  margin-top: 50px;
  /* Grid styles */
  display: grid;
  align-items: center;
  justify-content: center;
  grid-template-columns: repeat(auto-fit, minmax(140px, 1fr));
}
.flex-social-item{
  a{
    // width: 100%;
    transition: 0.5s;
    color: #FFFFFF;
    background: #30343F;
    border-radius: 4px;
    text-align: center;
    text-decoration: none;
    font-family: fontawesome;

    padding: 1rem;	
    margin: 1rem;
    line-height: 3.2rem;
    -o-transition:all 0.5s;
    -webkit-transition: all 0.5s;
    -moz-transition: all 0.5s;
    transition: all 0.5s;
    -webkit-font-smoothing: antialiased;
    span{
      padding-left: 5px;
    }
  }
}
a:hover {
  background: #d447b9;
  text-decoration: none;
}

/* font awesome icons */
.instagram:before {
	content: '\f16d';
	font-size: 18px;
}
.twitter:before {
	content:'\f099';
	font-size: 18px;
}

.github:before {
	content:'\f113';
	font-size: 18px;
}
.my-resume:before {
	content: '\f2c3';
	font-size: 16px;
}
.linkedin:before {
	content: '\f08c';
	font-size: 18px;
}
.description {
  padding: 1rem;
}
</style>
