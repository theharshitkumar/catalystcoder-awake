<template>
  <div id="post-page" class="page-wrapper post-page">
    <site-hero :title="title" :subtitle="subtitle" :image="featureImage">
      <span
        v-if="author && $siteConfig.posts.displayAuthor"
        class="author-wrapper"
      >
        <strong>Author:</strong> {{ author }}
      </span>
      <span v-if="date" class="date-wrapper">
        <strong>Published on:</strong> {{ date }}
      </span>
    </site-hero>
    <main-section :one-column-constrained="true">
	
      <template v-slot:default>
	  <script async src="https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js"></script>
<!-- sq ads -->
<ins class="adsbygoogle"
     style="display:block"
     data-ad-client="ca-pub-8385183705194513"
     data-ad-slot="5485579711"
     data-ad-format="auto"
     data-full-width-responsive="true"></ins>
<script>
     (adsbygoogle = window.adsbygoogle || []).push({});
</script>
	  <Adsense
    data-ad-client="ca-pub-8385183705194513"
    data-ad-slot="1234567890">
</Adsense>
        <div class="post-wrapper">
          <markdown :markdown="$store.state.content" />
		  <script async src="https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js"></script>
<ins class="adsbygoogle"
     style="display:block; text-align:center;"
     data-ad-layout="in-article"
     data-ad-format="fluid"
     data-ad-client="ca-pub-8385183705194513"
     data-ad-slot="8702221259"></ins>
<script>
     (adsbygoogle = window.adsbygoogle || []).push({});
</script>
		  <InArticleAdsense
    data-ad-client="ca-pub-8385183705194513"
    data-ad-slot="1234567890">
</InArticleAdsense>
          <div class="other-posts">
            <h6 class="subtitle is-size-4">
              Related Posts
            </h6>
            <!-- Related Posts -->
            <posts-grid :number="3" :category="category" :exclude="slug" />
			<script async src="https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js"></script>
<!-- sq ads -->
<ins class="adsbygoogle"
     style="display:block"
     data-ad-client="ca-pub-8385183705194513"
     data-ad-slot="5485579711"
     data-ad-format="auto"
     data-full-width-responsive="true"></ins>
<script>
     (adsbygoogle = window.adsbygoogle || []).push({});
</script><script async src="https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js"></script>
<!-- sq ads -->
<ins class="adsbygoogle"
     style="display:block"
     data-ad-client="ca-pub-8385183705194513"
     data-ad-slot="5485579711"
     data-ad-format="auto"
     data-full-width-responsive="true"></ins>
<script>
     (adsbygoogle = window.adsbygoogle || []).push({});
</script>
          </div>
          <disqus-comments :identifier="$route.params.singlePost" />
        </div>
      </template>
      <template v-slot:sidebar>
        <post-sidebar />
      </template>
    </main-section>
  </div>
</template>
<script>
import { mapState } from 'vuex'
import { setPageData, getFormattedDate } from '../helper'
// import 'highlight.js/styles/github.css'
import Markdown from '~/components/Markdown'
import PostSidebar from '~/components/PostSidebar'
export default {
  components: {
    Markdown,
    PostSidebar
  },
  computed: {
    ...mapState([
      'title',
      'subtitle',
      'featureImage',
      'underSubtitle',
      'author',
      'category',
      'slug'
    ]),
    date() {
      return getFormattedDate(this.$store.state.date)
    },
    url() {
      return `${process.env.URL}/${this.$route.fullPath}`
    }
  },
  fetch({ store, params }) {
    setPageData(store, { resource: 'post', slug: params.singlePost })
  }
}
</script>
<style scoped lang="scss">
.edit-post {
  margin-bottom: 20px;
}
</style>
