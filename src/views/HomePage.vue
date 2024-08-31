<template>

  <section class="intro">
    <div class="container">
      <div class="intro-row">
        <div class="intro-content">
          <p class="intro-text">Hi, I’m Almaz, a Full-Stack Web Developer with UX Designer background, a total tech geek and a perfectionist by nature.</p>
        </div>

        <div class="intro-portrait">
          <div class="intro-pic">
            <img :src="pointerImage" alt="" class="intro-pic-pointer">
            <img :src="myPhoto" alt="" class="intro-pic-photo">
          </div>
        </div>
      </div>
    </div>
  </section>

  <portfolio-section />


</template>

<script lang="ts">
import { defineComponent } from "vue";
import pointerImage from '@/assets/images/pointer.svg';
import myPhoto from '@/assets/images/me.jpg';
import PortfolioSection from "@/components/PortfolioSection.vue";

export default defineComponent({
  name: "HomePage",

  components: {
    PortfolioSection,
  },

  data() {
    return {
      pointerImage,
      myPhoto,
    };
  },
});
</script>

<style scoped>
  .intro-row {
    display: flex;
    align-items: center;
  }

  .intro-content {
    flex: 1;
    padding-top: 60px;
  }

  .intro-portrait {
    flex: 1;
    display: flex;
    justify-content: flex-end;
  }

  .intro-text {
    width: 546px;
    max-width: 100%;
    font-weight: 500;
    font-size: 48px;
    line-height: 1.4;
    letter-spacing: -0.01em;
  }

  .intro-pic {
    position: relative;
    width: 540px;
    margin: 0;
  }

  .intro-pic-photo {
    border-radius: 200px;
    display: block;
    width: 100%;
    margin: 0;
  }

  .intro-pic-pointer {
    position: absolute;
    width: 260px;
    bottom: 75%;
    right: 90%;
    animation: shake 2s infinite;
  }

  @keyframes shake {
    0% { transform: translate(0, 0); }
    25% { transform: translate(3px, 0); }
    50% { transform: translate(-3px, 0); }
    75% { transform: translate(3px, 0); }
    100% { transform: translate(0, 0); }
  }
</style>
