<template>
<header>
  <nav>
    <a href="#" id="logo">
      <img src="@/assets/images/logo.svg" alt="Logo" width="239">
    </a>

    <a href="#" id="tryItFree">Try It Free</a>
  </nav>
</header>

<!-- BUILDCOMMUNITY -->
<section class="buildCommunity">

  <div class="buildCommunity-started">

        <h1>Build The Community Your Fans Will Love</h1>
        <p class="buildCommunity_paragraph">Huddle re-imagines the way we build communities.You have a  voice, but so does your audience.Create connections with your   users as you engage in genuine discussion.</p>
      <Getstarted/>
      <div class="buildCommunity_banner">
        <img class="buildCommunity_banner__img" src="@/assets/images/screen-mockups.svg" alt="Mockups">
      </div>

      <div class="buildCommunity_stats">
          <div class="buildCommunity_stats_communities">
            <img class="buildCommunity_stats_communities__img" src="@/assets/images/icon-communities.svg" alt="Communities icon">
            <h2>1.4k+</h2>
            <p id="buildCommunity_stats__paragraph">Communities Formed</p>
          </div>
          
          <div class="buildCommunity_stats_messages">
            <img class="buildCommunity_stats_communities__img" src="@/assets/images/icon-messages.svg" alt="Message icon">
            <h2>2.7m+</h2>
            <p id="buildCommunity_stats__paragraph2">Messages Sent</p>
          </div>
      </div>

      
  </div>
</section>

<!-- GROWTOGETHER -->

<Wavepale/>

<!-- FLOWING CONVERSATIONS -->

<Flowing/>

<!-- USERS -->

<Users/>

<!-- READYBUILD -->
<Readybuild/>

<!-- SOCIAL -->
<Social/>
</template>

<script>
import Getstarted from "@/components/Getstarted.vue";
import Wavepale from "@/components/Growtogether.vue";
import Flowing from "@/components/Flowing.vue";
import Users from "@/components/Users.vue"
import Readybuild from "../components/Readybuild.vue"
import Social from "../components/Social.vue"
export default {
  components : {
    Getstarted,
    Wavepale,
    Flowing,
    Users,
    Readybuild,
    Social
}
}
</script>