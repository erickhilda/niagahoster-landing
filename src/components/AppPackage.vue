<template>
  <div class="section__wrapper">
    <b-container fluid="">
      <span class="section__title">Paket Hosting Singapura yang Tepat</span>
      <p class="section__subtitle">
        Diskon 40% + Domain dan SSL Gratis untuk Anda
      </p>
      <b-row align-h="center">
        <app-card-package
          v-for="(item, i) in packages"
          :key="`${i}`"
          :package-name="item.package_name"
          :real-price="item.real_price"
          :price="item.discount"
          :customer="item.customer_count"
          :disk-space="item.disk_space"
          :resource-power="item.resource_power"
          :bandwidth="item.bandwidth"
          :databases="item.database"
          :addon-domain="item.addon_domain"
          :backup="item.backup"
          :ssl="item.ssl"
          :email="item.email"
          :free-domain="item.free_domain"
          :name-server="item.name_server"
          :mail-protection="item.mail_protection"
          :support="item.support_service"
          :best-seller="item.is_best_seller"
        />
      </b-row>
    </b-container>
    <b-container class="section__wrapper">
      <p class="section__subtitle mb-4">
        Powerful dengan Limit yang Lebih Besar
      </p>
      <b-row align-h="center">
        <b-col cols="12" lg="4">
          <b-list-group>
            <b-list-group-item
              class="d-flex justify-content-between align-items-center"
            >
              <b-icon
                icon="check-circle"
                variant="success"
                scale="1.2"
                class="mr-2"
              />
              max execution time 300s
            </b-list-group-item>
            <b-list-group-item
              class="d-flex justify-content-between align-items-center"
            >
              <b-icon
                icon="check-circle"
                variant="success"
                scale="1.2"
                class="mr-2"
              />
              max execution time 300s
            </b-list-group-item>
            <b-list-group-item
              class="d-flex justify-content-between align-items-center"
            >
              <b-icon
                icon="check-circle"
                variant="success"
                scale="1.2"
                class="mr-2"
              />
              php memory limit 1024 MB
            </b-list-group-item>
          </b-list-group>
        </b-col>
        <b-col cols="12" lg="4">
          <b-list-group>
            <b-list-group-item
              class="d-flex justify-content-between align-items-center"
            >
              <b-icon
                icon="check-circle"
                variant="success"
                scale="1.2"
                class="mr-2"
              />
              post max size 128 MB
            </b-list-group-item>
            <b-list-group-item
              class="d-flex justify-content-between align-items-center"
            >
              <b-icon
                icon="check-circle"
                variant="success"
                scale="1.2"
                class="mr-2"
              />
              upload max filsize 128 MB
            </b-list-group-item>
            <b-list-group-item
              class="d-flex justify-content-between align-items-center"
            >
              <b-icon
                icon="check-circle"
                variant="success"
                scale="1.2"
                class="mr-2"
              />
              max input vars 2500
            </b-list-group-item>
          </b-list-group>
        </b-col>
      </b-row>
    </b-container>
  </div>
</template>

<script>
import AppCardPackage from "@/components/AppCardPackage";

export default {
  components: { AppCardPackage },
  data() {
    return {
      packages: []
    };
  },
  created() {
    this.getDataPackage();
  },
  methods: {
    async getDataPackage() {
      try {
        await fetch(
          "https://my-json-server.typicode.com/erhilds/niaga-price/package"
        )
          .then(response => response.json())
          .then(data => {
            this.packages = data;
          });
      } catch (error) {
        console.log(error);
      }
    }
  }
};
</script>
