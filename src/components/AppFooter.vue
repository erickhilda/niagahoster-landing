<template>
  <div class="bg-secondary">
    <b-container class="section__wrapper">
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
  </div>
</template>
