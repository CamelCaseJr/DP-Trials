<template>
  <div>
    <h6 class="text-grey-10 m-20">DP-Trials</h6>

    <div class=" row justify-content-center">
      <router-link
        class=" p-10 sidebar-btn d-flex  "
        to="/"
      >
        <i class="ms-10 me-10 flaticon-logout"></i>
        <span class="title fw-semibold ms-10 me-10 ">Contact</span>
      </router-link>

      <router-link
        class=" p-10 card-link-btn d-flex justify-self-center"
        to="/clients"
      >
        <i class="flaticon-logout"></i>
        <span class="title">Logout2</span>
      </router-link>

    </div>
  </div>
</template>


<script setup lang="ts">
</script>


<style scoped lang="sass">
@import 'src/css/quasar.variables.scss'
.sidebar-btn
  color: $grey-7
  border-radius: 10px
  width: 70%
  text-decoration: none


.sidebar-btn:hover
  background-color: $blue-1
  opacity: 75%
  color: $blue-9

.router-link-active
  background-color: $blue-6
  color: white

.router-link-active:hover
  background-color: $blue-6
  color: white
  opacity: 100%



</style>
