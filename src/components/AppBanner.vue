<template>
  <div class="border-bottom">
    <b-container>
      <b-row align-content="start" class="hero">
        <b-col cols="" class="text-left">
          <h3 class="hero__title">PHP Hosting</h3>
          <h3 class="hero__subtitle">
            Cepat, handal, penuh dengan modul PHP yang anda butuhkan
          </h3>
          <ul class="list-unstyled">
            <b-media tag="li" v-for="item in advantageList" :key="item">
              <h5 class="mb-1 hero__list">
                <b-icon
                  icon="check-circle"
                  variant="success"
                  scale="1.2"
                  class="mr-2"
                />
                {{ item }}
              </h5>
            </b-media>
          </ul>
        </b-col>
        <b-col class="text-right">
          <b-img
            width="420"
            :src="
              require('../assets/svg/illustration banner PHP hosting-01.svg')
            "
          />
        </b-col>
      </b-row>
    </b-container>
  </div>
</template>

<script>
export default {
  data() {
    return {
      advantageList: [
        "Solusi PHP untuk performa query yang lebih cepat",
        "Konsumsi memory yang lebih rendah",
        "Support PHP 5.3, PHP 5.4, PHP 5.5, PHP 5.6, PHP 7",
        "Fitur enkripsi ionCube dan Zend Guard Loaders"
      ]
    };
  }
};
</script>

<style lang="scss">
.hero {
  padding: 70px 0px;
}

.hero__title {
  font-family: "Montserrat", sans-serif;
  font-weight: 700;
  color: #000000;
  margin-bottom: 14px;
}

.hero__subtitle {
  font-family: "Montserrat", sans-serif;
  font-weight: 300;
  color: #000000;
  margin-bottom: 20px;
}

.hero__list {
  font-family: "Montserrat", sans-serif;
  font-weight: 300;
  font-size: 20px;
}
</style>
