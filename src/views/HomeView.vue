<template>
  <div
    id="Home"
    class="flex flex-col h-screen"
  >
    <div class="m-3 mb-auto">

      <div class="my-16">
        <img
          alt=""
          width="150"
          src="img/uber/uber2.svg"
        >
      </div>
      <div class="grid grid-cols-2 gap-3 my-3">
        <ServiceSelectLarge
          text="Ride"
          image-width="70"
          image="ride"
        />
        <ServiceSelectLarge
          text="Food"
          image-width="70"
          image="food"
          promo="true"
        />
      </div>
      <div class="grid grid-cols-4 gap-3 my-3">
        <ServiceSelectSmall
          text="2 Wheels"
          image="2wheels"
        />
        <ServiceSelectSmall
          text="Transit"
          image="Transit"
        />
        <ServiceSelectSmall
          text="Reserve"
          image="reserve"
        />
        <ServiceSelectSmall
          text="Travel"
          image="travel"
        />
      </div>

      <div
        class="
          w-full
          bg-custom-color
          h-14
          rounded-full
          flex
          items-center
          p-3
        "
      >
        <MagnifyIcon
          :size="40"
        />
        <div class="ml-3 text-xs font-semibold text-gray-700">
          Enter pick-up point
        </div>

      </div>

    </div>
    <FooterNav/>
  </div>
</template>

<script setup>
import ServiceSelectLarge from '../components/ServiceSelectLarge.vue'
import ServiceSelectSmall from '../components/ServiceSelectSmall.vue'
import FooterNav from '../components/FooterNav.vue'

import MagnifyIcon from 'vue-material-design-icons/Magnify.vue'

</script>

<style lang="scss">

#Home{
  .bg-custom-color{
    background-color: rgb(237, 237, 237);
  }
}
</style>
