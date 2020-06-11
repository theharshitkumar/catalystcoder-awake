<template>
  <footer class="site-footer">
    {{ $siteConfig.siteName }} &copy; {{ new Date().getFullYear() }} - All
    Rights Reserved
    <br />
    <a href="https://www.linkedin.com/in/harshitkumar197/"> Made with <span style="color: #e25555;">&#9829;</span> By HK </a>
	<div class="social">
	<h2>Follow Us</h2>
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
  </footer>
</template>

<script>
export default {
  name: 'SiteFooter'
}
</script>

<style scoped>
footer {
  background: #eee;
  padding: 20px 10px;
  text-align: center;
  transition: 0.5s ease all;
}
social{
  font-size: 20px;
  margin: 20px 20px 20px 20px;

}

.social a i {
    padding: 0px 20px 0px 10px;
    font-size: 35px;
}
</style>
