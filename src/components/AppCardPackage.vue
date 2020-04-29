<template>
  <b-card
    :border-variant="bestSeller ? 'primary' : 'outline-secondary'"
    no-body
    style="max-width: 20rem;"
    class="my-2"
  >
    <b-list-group flush>
      <b-list-group-item :active="bestSeller">
        {{ packageName }}
      </b-list-group-item>
      <b-list-group-item :active="bestSeller">
        <p>
          <s> Rp. {{ realPrice }} </s>
        </p>
        <h3>
          <span class="__sign">Rp.</span>
          <span class="__price">{{ price }}</span>
        </h3>
      </b-list-group-item>
      <b-list-group-item :active="bestSeller">
        <strong>{{ customer }}</strong>
        Pengguna Terdaftar
      </b-list-group-item>
    </b-list-group>

    <b-card-body>
      <ul class="list-unstyled">
        <li v-if="resourcePower">
          <p>
            <strong>{{ resourcePower }}</strong> Resource Power
          </p>
        </li>
        <li v-if="diskSpace">
          <p>
            <strong>{{ diskSpace }}</strong> Disk Space
          </p>
        </li>
        <li v-if="bandwidth">
          <p>
            <strong>{{ bandwidth }}</strong> bandwidth
          </p>
        </li>
        <li v-if="email">
          <p>
            <strong>{{ email }}</strong> POP3 Email
          </p>
        </li>
        <li v-if="databases">
          <p>
            <strong>{{ databases }}</strong> Databases
          </p>
        </li>
        <li v-if="addonDomain">
          <p>
            <strong>{{ addonDomain }}</strong> Addon Domain
          </p>
        </li>
        <li v-if="backup">
          <p>
            <strong>{{ backup }}</strong> Backup
          </p>
        </li>
        <li v-if="freeDomain">
          <p>
            <strong>{{ freeDomain }}</strong> Selamanya
          </p>
        </li>
        <li v-if="ssl">
          <p>
            <strong>{{ ssl }}</strong> Gratis Selamanya
          </p>
        </li>
        <li v-if="nameServer">
          <p>
            <strong>{{ nameServer }}</strong> Name Server
          </p>
        </li>
        <li v-if="support">
          <p>Prioritas Layanan Support</p>
        </li>
        <li v-if="mailProtection">
          <p>
            <strong>{{ mailProtection }}</strong> Mail Protection
          </p>
        </li>
      </ul>
    </b-card-body>
    <template v-slot:footer>
      <b-button pill="" :variant="bestSeller ? 'primary' : 'outline-secondary'">
        Pilih Sekarang
      </b-button>
    </template>
  </b-card>
</template>

<script>
// eslint-disable-next-line vue/valid-v-bind
export default {
  props: {
    packageName: {
      type: String,
      default: ""
    },
    realPrice: {
      type: String,
      default: ""
    },
    price: {
      type: String,
      default: ""
    },
    customer: {
      type: String,
      default: ""
    },
    resourcePower: {
      type: String,
      default: ""
    },
    diskSpace: {
      type: String,
      default: ""
    },
    bandwidth: {
      type: String,
      default: ""
    },
    databases: {
      type: String,
      default: ""
    },
    addonDomain: {
      type: String,
      default: ""
    },
    backup: {
      type: String,
      default: ""
    },
    ssl: {
      type: String,
      default: ""
    },
    email: {
      type: String,
      default: ""
    },
    freeDomain: {
      type: String,
      default: ""
    },
    nameServer: {
      type: String,
      default: ""
    },
    mailProtection: {
      type: String,
      default: ""
    },
    support: {
      type: String,
      default: ""
    },
    bestSeller: {
      type: Boolean,
      default: false
    }
  }
};
</script>

<style lang="scss">
.__sign {
  font-size: 37.5%;
  padding: 10px 10px 0 0;
}

.__price {
  font-weight: 700;
}

.__extra {
  padding-left: 10px;
  position: relative;
  text-align: left;
}

.__cents {
  font-size: 31.25%;
}

.__frequency {
  bottom: 0;
  font-size: 12px;
  left: 10px;
  line-height: 1.2;
  position: absolute;
}
</style>
