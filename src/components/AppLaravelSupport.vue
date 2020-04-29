<template>
  <div>
    <div class="border-bottom mt-5">
      <b-container>
        <p class="section__subtitle mb-4">
          Mendukung Penuh framework Laravel
        </p>
        <b-row align-content="start">
          <b-col cols="12" lg="6" class="text-left">
            <h5 class="section__intro">
              Tidak perlu menggunkan dedicated server ataupun VPS yang mahal.
              Layanan PHP hosting kami mendukung penuh framework favorit Anda.
            </h5>
            <ul class="list-unstyled">
              <b-media tag="li" v-for="item in advantageList" :key="item">
                <h5 class="mb-1 section__content__list">
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
            <small>
              Nb: Composer dan SSH hanya tersedia pada paket Personal dan
              Bisnis.
            </small>
            <b-button variant="primary" pill="" class="mt-2">
              Pilih Hosting Anda
            </b-button>
          </b-col>
          <b-col cols="12" class="text-right" lg="6">
            <b-img
              width="450"
              fluid=""
              :src="
                require('../assets/svg/illustration banner support laravel hosting.svg')
              "
            />
          </b-col>
        </b-row>
      </b-container>
    </div>
    <b-container class="section__wrapper">
      <p class="section__subtitle mb-4">
        Modul Lengkap untuk Menjalankan Aplikasi PHP Anda.
      </p>
      <b-row align-h="center">
        <b-col
          class="mx-3"
          cols="12"
          lg="2"
          v-for="(item, index) in modulList"
          :key="index"
        >
          <ul class="list-unstyled">
            <li class="text-left" v-for="modul in item.modul1" :key="modul">
              {{ modul }}
            </li>
          </ul>
        </b-col>
      </b-row>
      <b-button pill="" variant="outline-secondary" class="mt-3">
        Selengkapnya
      </b-button>
    </b-container>
    <b-container>
      <b-row align-content="start" align-h="center">
        <b-col cols="12" lg="5" class="text-left">
          <h3 class="section__intro">
            Linux Hosting yang Stabil dengan Teknologi LVE
          </h3>
          <p>
            SuperMicro <strong>Intel Xeon 24-Cores</strong> server dengan RAM
            <strong>128 GB</strong> dan teknologi
            <strong>LVE CloudLinux</strong> untuk stabilitas server Anda.
            Dilengkapi dengan <strong>SSD</strong> untuk kecepatan
            <strong>MySQL</strong> dan caching. Apache load balancer berbasis
            LIghtSpeed Technologies, <strong>CageFS</strong> security,
            <strong>Raid-10</strong>
            protection dan auto backup untuk keamanan website PHP Anda.
          </p>
          <b-button variant="primary" pill="" class="my-4">
            Pilih Hosting Anda
          </b-button>
        </b-col>
        <b-col align-self="end" cols="12" class="text-right" lg="6">
          <b-img
            width="450"
            fluid=""
            :src="require('../assets/images/Image support.png')"
          />
        </b-col>
      </b-row>
    </b-container>
    <b-container class="bg-light" fluid="">
      <b-row
        align-h="center"
        align-v="center"
        align-content="center"
        class="py-2"
      >
        <b-col cols="12" lg="6" align-self="center">
          <p>Bagikan jika anda menyukai halaman ini</p>
        </b-col>
        <b-col cols="12" lg="6"> </b-col>
      </b-row>
    </b-container>
    <div class="bg-primary">
      <b-container>
        <b-row align-h="center" class="py-4">
          <b-col cols="12" lg="6">
            <h5 class="section__intro" style="color: #ffffff;">
              Perlu <strong>BANTUAN?</strong> Hubungi kami:
              <strong>0274-5305505</strong>
            </h5>
          </b-col>
          <b-col cols="12" lg="6">
            <b-button variant="outline-light" pill="">
              <b-icon icon="chat-dots-fill" />
              Live Chat
            </b-button>
          </b-col>
        </b-row>
      </b-container>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      advantageList: [
        "Install Laravel 1 klik dengan Softaculous Installer.",
        "Mendukung PHP Mcrypt, phar, mbstring, json, dan fileinfo.",
        "Tersedia composer dan SSH untuk menginstall packages pilihan anda."
      ],
      modulList: [
        {
          modul1: [
            "IcePHP",
            "apc",
            "apcu",
            "apm",
            "ares",
            "bcmath",
            "bcompiler",
            "big_int",
            "bitset",
            "bloomy",
            "bz2_filter",
            "clamav",
            "coin_acceptor",
            "crack",
            "dba"
          ]
        },
        {
          modul1: [
            "http",
            "huffman",
            "idn",
            "igbinary",
            "imagick",
            "imap",
            "include",
            "inotify",
            "interbase",
            "intl",
            "ioncube_loader",
            "ioncube_loader_4",
            "jsmin",
            "json",
            "ldap"
          ]
        },
        {
          modul1: [
            "nd_pdo_mysql",
            "oauth",
            "oci8",
            "odbc",
            "opcache",
            "pdf",
            "pdo",
            "pdo_pdlib",
            "pdo_firebird",
            "pdo_mysql",
            "pdo_odbc",
            "pdo_pgsql",
            "pdo_sqlite",
            "pgsql",
            "phalcon"
          ]
        },
        {
          modul1: [
            "stats",
            "stem",
            "stomp",
            "suhosin",
            "sybase_ct",
            "sysvmsg",
            "sysvsem",
            "sysvshm",
            "tidy",
            "timezonedb",
            "trader",
            "translit",
            "uploadprogress",
            "uri_template",
            "uuid"
          ]
        }
      ]
    };
  }
};
</script>

<style lang="scss">
.section__wrapper {
  padding: 70px 0px 0px 0px;
}

.section__intro {
  font-family: "Montserrat", sans-serif;
  font-weight: 300;
  color: #4c4c4c;
  margin-bottom: 17px;
}

.section__content__list {
  font-family: "Montserrat", sans-serif;
  font-weight: 300;
  font-size: 16px;
}
</style>
