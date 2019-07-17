<template>
  <section class="bg-light" id="portfolio">
    <div class="container">
      <div class="row">
        <div class="col-lg-12 text-center">
          <h2 class="section-heading text-uppercase">Portfolio</h2>
          <h3 class="section-subheading text-muted">Lorem ipsum dolor sit amet consectetur.</h3>
        </div>
      </div>
      <div class="row">
        <div
          class="col-md-4 col-sm-6 portfolio-item"
          v-for="(obj, key) in portfolioJSON"
          :key="key"
        >
          <a class="portfolio-link" data-toggle="modal" href="#portfolioModal2">
            <div class="portfolio-hover">
              <div class="portfolio-hover-content">
                <i class="fas fa-plus fa-3x"></i>
              </div>
            </div>
            <img class="img-fluid" src="img/portfolio/02-thumbnail.jpg" alt />
          </a>
          <div class="portfolio-caption">
            <h4>{{ obj.caption }}</h4>
            <p class="text-muted">{{ obj.title }}</p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data: () => ({
    portfolioJSON: [
      {
        img: "/something/random/img.jpg",
        caption: "ILWYS Tour",
        title: "Somebody else Stage"
      },
      {
        img: "/something/random/img.jpg",
        caption: "Lyrics Video",
        title: "If I Believe you"
      },
      {
        img: "/something/random/img.jpg",
        caption: "Acoustic Setup",
        title: "Jesus Christ 2005 God Bless America"
      },
      {
        img: "/something/random/img.jpg",
        caption: "Photo Set",
        title: "UK tour"
      },
      {
        img: "../assets/img/thesound.jpg",
        caption: "Lyrics Video",
        title: "The Sound"
      },
      {
        img: "/something/random/img.jpg",
        caption: "Tour visuals",
        title: "I like America and America likes me"
      }
    ]
  })
};
</script>

<style lang="css">
</style>