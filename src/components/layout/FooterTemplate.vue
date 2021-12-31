<template>
  <div id="footer-template">

  <div class="footer">
    <div class="footer-sec">
      <div class="logo">
        <a href="#page-top">
          <!-- logoBlackWhite class="footer-logo" /-->
          <img
            class="footer-logo"
            :src="require(`../../assets/logo_white.png`)"
            alt="Fragcolor Logo White"   
          />
        </a>
      </div>

      <!-- div class="footer-menu">
        <router-link to="/technology" class="footerMenuStyle"> Technology </router-link>
      </div -->

      <!-- div class="media-icons">
        <a href="https://twitter.com/fragcolor" target="_blank">
          <twitter class="icon" />
        </a>
        <a href="https://discord.fragcolor.com/" target="_blank">
          <discord class="icon" />
        </a>
        <a href="https://t.me/fragcolor" target="_blank">
          <telegram class="icon" />
        </a>
        <a href="https://medium.com/@fragcolor" target="_blank">
          <medium class="icon" />
        </a>
        <a href="https://www.linkedin.com/company/fragcolor/" target="_blank">
          <linkedIn class="icon" />
        </a>
        <a href="https://github.com/fragcolor-xyz" target="_blank">
          <github class="icon" />
        </a>
        <a href="https://angel.co/company/fragcolor" target="_blank">
          <angelList class="icon" />
        </a>
      </div -->

      <div class="footer-submenu">
        <p class="footerMenuStyle"> info@fragcolor.com </p>
      </div>

      <div class="footer-copyright">
        <p>Copyright © 2021 Fragcolor Pte. Ltd.</p>
      </div>
    </div>
  </div>


    <!--div class="content">
      <div class="links">
        <a
          href="https://github.com/DOkwufulueze/eth-vue"
          target="_blank"
          class="link2"
          >Github</a
        >
        <span class="divider" />
        <a href="http://danielokwufulueze.com" target="_blank" class="link3"
          >www</a
        >
      </div>

      <div class="copyleft">
        <div class="text">
          Copyleft <span class="copyleft-resource" /> 2017
          <a href="https://danielokwufulueze.com" class="link2"
            >Daniel Okwufulueze</a
          >.
        </div>
      </div>

      <div class="social">
        <a
          href="https://facebook.com/DOkwufulueze"
          target="_blank"
          class="facebook"
        />
        <a
          href="https://twitter.com/dokwufulueze"
          target="_blank"
          class="twitter"
        />
      </div>
    </div-->

  </div>
</template>

<script>
export default {
  name: "FooterTemplate"
};
</script>

<style scoped>
#footer-template {
  width: 100%;
  background: black;
  color: #1d1e1f;
  /* height: 150px; */
  height: 300px;
  position: relative;
  bottom: 0;
  min-width: 700px;
  border-top: 1px solid #333;
  top: 200vh;
}

.footer-logo {
  width: 200px;
  margin-top: 30px;
  margin-left: 50px;
}

.footer {
  width: 100vw;
}

.footer p {
  color: white;
}

.footer-submenu {
  float: right;
  margin-right: 50px;
  display: inline-block;
}


.footer-copyright {
  text-align: center;
  bottom: 20px;
  position: relative;
  top: 100px;
}

.footer-copyright p {
  width: 100vw;
  display: inline-block;
}








.content {
  height: 100%;
  max-width: 920px;
  margin: auto;
  text-align: center;
  padding: 50px 0px 10px 0px;
}

.links {
  clear: both;
  height: 20px;
  margin-bottom: 30px;
}

.links a {
  color: inherit;
  text-decoration: none;
}

.divider {
  color: inherit;
}

.divider:before {
  content: "|";
}

.copyright {
  clear: both;
  height: 20px;
  font-size: 14px;
}

.copyleft-resource {
  background: url("../../../static/images/copyleft.png") no-repeat;
  height: 20px;
  width: 20px;
  display: inline-block;
  background-size: contain;
}

.social {
  clear: both;
  height: 20px;
  float: right;
  position: relative;
  top: -39px;
}

.facebook {
  display: inline-block;
  width: 20px;
  height: 20px;
  background: url("../../../static/images/Facebook.png") no-repeat;
  background-size: contain;
}

.twitter {
  display: inline-block;
  width: 20px;
  margin: 0px 0px 0px 30px;
  height: 20px;
  background: url("../../../static/images/twitter.png") no-repeat;
  background-size: contain;
}
</style>
