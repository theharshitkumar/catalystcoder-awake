<template>
  <div id="contact-page" class="page-wrapper contact-page content-page">
    <site-hero
      title="Contact Us"
      subtitle="We are here to help you"
      image="/uploads/contact-hero.jpg"
    ></site-hero>
    <main-section theme="sidebar-right">
      <template v-slot:default>
        <div class="tile is-ancestor">
          <div class="tile is-parent">
            <article class="tile is-child box">
              <p class="title">
                Hi!
              </p>
              <p class="subtitle">
                What can I do for you?
              </p>
              <figure class="image is-1by1 ">
                <opti-image
                  :src="require('~/assets/uploads/contact-person.jpg').src"
                  :srcset="
                    require('~/assets/uploads/contact-person.jpg').srcSet
                  "
                />
              </figure>
              <br />
              <div class="content">
                <p>
                  Hi I am Harshit.<br>
				  A tech enthusiast<br> 
				  and a Web Developer.<br>
				  I am still on learning process<br>
				  and exploring new things daily<br>
				  I made this blog for the sole purpose to share my knowledge with the world for free<br>
				  Feel free to surf on my blog and YouTube channel<br>
				  
                </p>
              </div>
            </article>
          </div>
          <div class="tile is-parent is-8">
            <article class="tile is-child box">
			<div class="contact">
              <iframe src="https://docs.google.com/forms/d/e/1FAIpQLSdp4hoIvqfk6L0UzeUU9D8-i3Pt2PyRxvD1FlkYNhL-yoiATQ/viewform?embedded=true" width="640" height="905" frameborder="0" marginheight="0" marginwidth="0">Loading…</iframe>
			  <p> Please give me 4-5 business days to get back to you </p>
			  </div>
            </article>
          </div>
        </div>
      </template>
      <template v-slot:sidebar>
        <h3 class="subtitle is-4">
          Latest Posts
        </h3>
        <!-- Latest Posts -->
        <posts-grid :per-row="1" :number="2" />
      </template>
    </main-section>
  </div>
</template>
<script>
import ContactForm from '~/components/ContactForm'
export default {
  head() {
    return {
      title: `Contact | ${this.$siteConfig.siteName}`
    }
  },
  components: { ContactForm }
}
</script>
<style>
.contact iframe{
height:905px!important;

}
.freebirdSolidBackground{
background-color:white!important;
}
.m2 .freebirdFormviewerViewNavigationPasswordWarning{
display:none!important;
}

.freebirdDisclaimerColor, .freebirdDisclaimerColor a{
display:none!important;
}
.freebirdFormviewerViewFooterEmbeddedBackground {
    display: none!important;
}
.freebirdSolidBackground {
     background-color: white!important;
    color: rgba(255, 255, 255, 1);
}

</style>