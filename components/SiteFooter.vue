<template>
  <footer class="site-footer">
    {{ $siteConfig.siteName }} &copy; {{ new Date().getFullYear() }} - All
    Rights Reserved
    <br />
    <a href="https://www.linkedin.com/in/harshitkumar197/"> Made with <span style="color: #e25555;">&#9829;</span> By HK </a>
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
</style>
