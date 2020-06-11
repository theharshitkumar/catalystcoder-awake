<template>
  <div id="about-page" class="page-wrapper about-page content-page">
    <site-hero
      title="About Us"
      subtitle="We like to think that we are AWESOME!"
      image="/uploads/about-hero.jpg"
    ></site-hero>
    <main-section theme="sidebar-right">
      <template v-slot:default>
        <div class="content">
          <h3>About Catalyst Coder</h3>
          <p>
            <strong>
              Catalyst Coder is a group of people came together to spread the knowledge they have with the society.
            </strong>
			<br>
			<br>
			<br>
			<subtitle>
			The purpose behind the foundation of the group <code>Catalyst Coder</code> was to share knowledge which<br>
			we learn here with the others for free. So the people don't have to face the problems<br> which we faced while learning the same thing<br>
			<h4>#togetherwelearn</h4>
			<h4>#togetherwegrow</h4>
			<br>
			<br>
			<br>
			<br>
			<br>
			<br>
			<h3>Whats App and Telegram groups will be formed soon </h3>
			<h2>Stay Tuned for that!!!!</h2>
			</subtitle>
          </p>
        </div>

        <div class="tile is-ancestor">
          <div class="tile is-parent">
            
          </div>
          <div class="tile is-parent">
            
          </div>
          <div class="tile is-parent">
            
          </div>
        </div>
      </template>

      <template v-slot:sidebar>
        <h3 class="subtitle is-4">
          Latest Posts
        </h3>
        <posts-grid :per-row="1" :number="2" />
      </template>
    </main-section>
  </div>
</template>
<script>
import QuoteCard from '~/components/cards/QuoteCard'
export default {
  head() {
    return {
      title: `About | ${this.$siteConfig.siteName}`
    }
  },
  components: { QuoteCard }
}
</script>
