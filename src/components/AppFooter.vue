<template>
    <footer class="footer">
  <div class="content has-text-centered">
    <h1>
      Download Pitch-Match Now
    </h1>
    <p>
      Available for all iOS and Android devices
    </p>
    <p>
      <router-link class="badge" to="/en">
                  <img alt="App Store Badge" src="./../assets/app-store-badge.png"
                  width="150" height="auto">
      </router-link> 
     <router-link class="badge" to="/en">
        <img alt="App Store Badge" src="./../assets/google-play-badge.png"
        width="150" height="auto">
      </router-link> 
    </p>
    <h4>
      2020 Pitch-Match &#9917All rights reserved
    </h4>
  </div>
</footer>
</template>

<script>
export default {
}

</script>

<style scoped>

.footer {
  background-color:rgb(36, 34, 34);
  padding: 3rem 1.5rem 1rem !important;
}

 .footer h1 {
   color:#ffffff;
 } 

 .footer p {
   color:#ffffff;
   font-size: 22px;
   font-weight: lighter;
 }


.badge {
  padding-right: 16px;
}

.footer h4 {
  font-size: 13px;
  color: floralwhite;
  font-weight: 300;
}

</style>