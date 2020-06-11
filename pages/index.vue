<template>
  <div id="home-page" class="page-wrapper home-page">
    <site-hero :title="title" :subtitle="subtitle" :image="featureImage">
	<div class="social-main">
	<a href="https://www.youtube.com/channel/UCOyYK29kVXQvknRwdW_3-YQ" target="_blank"><i class="fab fa-youtube" data-v-0efc0558="" aria-hidden="true" style="
    padding: 0px 20px 0px 10px;
    font-size: 35px;
"></i></a>
	<a href="https://www.instagram.com/catalystcoder/" target="_blank"><i class="fab fa-instagram" data-v-0efc0558="" aria-hidden="true" style="
    padding: 0px 20px 0px 10px;
    font-size: 35px;
"></i></a>
	<a href="https://twitter.com/catalyst_coder" target="_blank"><i class="fab fa-twitter" data-v-0efc0558="" aria-hidden="true" style="
    padding: 0px 20px 0px 10px;
    font-size: 35px;
"></i></a>
	</div>
      <button
        v-if="$siteConfig.newsletter.on"
        class="button is-primary"
        @click="$eventBus.$emit('modal-triggered', 'newsletter-modal')"
      >
        Subscribe To Newsletter
      </button>
	  
    </site-hero>
    <main-section theme="one-column">
      <template v-slot:default>
        <!-- All Posts -->
        <posts-grid />
      </template>
      <template v-slot:sidebar>
        Nothing here
      </template>
    </main-section>
    <news-letter-form-modal />
  </div>
</template>

<script>
import { mapState } from 'vuex'
import { setPageData } from '../helper'
import NewsLetterFormModal from '~/components/NewsLetterFormModal'

export default {
  name: 'HomePage',
  head() {
    return {
      title: `Home | ${this.$siteConfig.siteName}`
    }
  },
  components: {
    NewsLetterFormModal
  },
  computed: {
    ...mapState(['title', 'subtitle', 'featureImage'])
  },
  fetch({ store, params }) {
    setPageData(store, { slug: 'home' })
  }
}
</script>

<style>
.home-page .under-subtitle {
  border-top: none;
}
.social-main a i{
font-size:25px;
padding: 0px 20px 10px 10px;

}
</style>
