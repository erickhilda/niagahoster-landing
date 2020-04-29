<template>
  <b-container fluid="">
    <b-row align-h="center">
      <p class="section__subtitle">Powerful dengan Limit yang Lebih Besar</p>
    </b-row>
    <b-row align-h="center">
      <b-col cols="12" lg="3" class="mx-2">
        <b-img
          :src="require('../assets/svg/icon PHP Hosting_PHP Semua Versi.svg')"
          alt="service-icon"
          fluid=""
          width="56"
        />
        <h5 class="content__title">PHP Semua Versi</h5>
        <p class="content__desc">
          Pilih dari PHP 5.3 s/d PHP 7. Ubah sesuka anda!
        </p>
      </b-col>
      <b-col cols="12" lg="3" class="mx-2">
        <b-img
          :src="require('../assets/svg/icon PHP Hosting_My SQL.svg')"
          alt="service-icon"
          fluid=""
          width="56"
        />
        <h5 class="content__title">MySQL versi 5.6</h5>
        <p class="content__desc">
          Nikmati MySQL versi terbaru, tercepat, dan kaya akan fitur.
        </p>
      </b-col>
      <b-col cols="12" lg="3" class="mx-2">
        <b-img
          :src="require('../assets/svg/icon PHP Hosting_CPanel.svg')"
          alt="service-icon"
          fluid=""
          width="56"
        />
        <h5 class="content__title">Panel Hosting cPanel</h5>
        <p class="content__desc">
          Kelola Website dengan panel canggih yang familiar dengan hari Anda.
        </p>
      </b-col>
      <b-col cols="12" lg="3" class="mx-2">
        <b-img
          :src="require('../assets/svg/icon PHP Hosting_garansi uptime.svg')"
          alt="service-icon"
          fluid=""
          width="56"
        />
        <h5 class="content__title">Garansi Uptime 99.9%</h5>
        <p class="content__desc">
          Data center yang mendukung kelangsungan website Anda 24/7.
        </p>
      </b-col>
      <b-col cols="12" lg="3" class="mx-2">
        <b-img
          :src="require('../assets/svg/icon PHP Hosting_InnoDB.svg')"
          alt="service-icon"
          fluid=""
          width="56"
        />
        <h5 class="content__title">Database InnoDB Unlimited</h5>
        <p class="content__desc">
          Jumlah dan ukuran database yang tumbuh sesuai kebutuhan Anda.
        </p>
      </b-col>
      <b-col cols="12" lg="3" class="mx-2">
        <b-img
          :src="require('../assets/svg/icon PHP Hosting_My SQL remote.svg')"
          alt="service-icon"
          fluid=""
          width="56"
        />
        <h5 class="content__title">Wilcard Remote MySQL</h5>
        <p class="content__desc">
          Mendukung s/d 25 max_user_connections dan 100 max_connections
        </p>
      </b-col>
    </b-row>
  </b-container>
</template>

<style lang="scss">
.content__title {
  font-family: "Montserrat", sans-serif;
  font-weight: 700;
  color: #4c4c4c;
  font-size: 18px;
}

.content__desc {
  font-family: "Montserrat", sans-serif;
  font-weight: 500;
  color: #4c4c4c;
  font-size: 13px;
}
</style>
