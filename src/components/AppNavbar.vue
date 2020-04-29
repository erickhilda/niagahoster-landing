<template>
  <div>
    <b-navbar toggleable="lg">
      <b-collapse is-nav>
        <b-container>
          <b-navbar-nav small="">
            <b-nav-item>
              <b-icon icon="bookmark-fill" variant="primary" />
              Gratis Ebook 9 Cara Cerdas Menggunakan Domain
              <b-icon icon="x" variant="danger" />
            </b-nav-item>
          </b-navbar-nav>
          <b-navbar-nav small="" class="ml-auto">
            <b-nav-item
              v-for="(item, index) in serviceMenu"
              :key="`menu_${index}`"
              href="#"
            >
              <b-icon :icon="item.icon" />
              {{ item.text }}
            </b-nav-item>
          </b-navbar-nav>
        </b-container>
      </b-collapse>
    </b-navbar>
    <b-navbar
      toggleable="lg"
      type="light"
      variant=""
      class="border-bottom border-top"
    >
      <b-container class="my-3">
        <b-navbar-brand href="#" toggleable="lg">
          <b-img-lazy
            src="https://www.niagahoster.co.id/blog/wp-content/uploads/2018/04/logo-blog.png"
            alt="niagahoster-logo"
            width="240"
          />
        </b-navbar-brand>

        <b-navbar-toggle target="nav-collapse" />

        <b-collapse id="nav-collapse" is-nav>
          <!-- Right aligned nav items -->
          <b-navbar-nav class="ml-auto">
            <b-nav-item
              v-for="(item, index) in navigationMenu"
              :key="`menu_${index}`"
              href="#"
              class="mx-1"
            >
              {{ item.text }}
            </b-nav-item>
          </b-navbar-nav>
        </b-collapse>
      </b-container>
    </b-navbar>
  </div>
</template>

<script>
export default {
  data() {
    return {
      navigationMenu: [
        { text: "Hosting", url: "#" },
        { text: "Domain", url: "#" },
        { text: "Server", url: "#" },
        { text: "Website", url: "#" },
        { text: "Afiliasi", url: "#" },
        { text: "Promo", url: "#" },
        { text: "Pembayaran", url: "#" },
        { text: "Review", url: "#" },
        { text: "Kontak", url: "#" },
        { text: "Blog", url: "#" }
      ],
      serviceMenu: [
        { text: "0274-5305505", url: "#", icon: "phone" },
        { text: "Live Chat", url: "#", icon: "chat-dots-fill" },
        { text: "Member Area", url: "#", icon: "people-circle" }
      ]
    };
  }
};
</script>
