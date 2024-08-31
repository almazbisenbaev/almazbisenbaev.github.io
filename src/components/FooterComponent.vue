<template>
  
  <section id="contact" class="section">
    <div class="container container-narrow container-padding">

      <div class="text-center"></div>

      <!-- <div class="cinfo">
        <div class="cinfo-title">Let's talk business</div>
        <div class="cinfo-items">
          <div class="cinfo-item">
            <a
              href="https://t.me/almazbisenbaev"
              target="_blank"
              rel="noopener noreferrer"
              >Telegram</a
            >
          </div>
          <div class="cinfo-item">
            <a
              href="https://www.linkedin.com/in/almazbisenbaev/"
              target="_blank"
              rel="noopener noreferrer"
              >Linkedin</a
            >
          </div>
        </div>
      </div> -->
      
    </div>
  </section>

</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "FooterComponent",
});
</script>

<style scoped>


.cinfo {
  display: flex;
  justify-content: space-between;
}

.cinfo a {
  color: #b5b0b8;
}

.cinfo a:hover,
.cinfo a:focus {
  color: #fff;
}

.cinfo-title {
  opacity: 0.75;
}

.cinfo-item {
  font-weight: 500;
  margin-bottom: 4px;
}

@media (max-width: 576px) {
  .cinfo-title {
    flex: 1.5;
  }

  .cinfo-items {
    flex: 1;
  }
}

</style>
