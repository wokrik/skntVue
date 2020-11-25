<template>
    <div class="tarif" :data-id="index">
      <h2 class="tarif__name">Тариф "{{ name }}"</h2>
      <div :class="index" class="tariff__info">
        <div class="tarif__speed">
<!--          -->
        </div>
<!--        <div class="tarif__prices">-->
<!--          <?echo(min($prices))?> &#8213 <?echo(max($prices) . $currency . "/мес")?>-->
<!--        </div>-->
        <div class="tarif__options">
          free options here
        </div>
        <i class="tarif__next-screen-btn arrow arrow_right"></i>
        <div class="tarif__more-info">
          <a href="" target="_blank" class="tarif__link">узнать подробнее на сайте www.sknt.ru</a>
        </div>+

      </div>
    </div>
</template>

<script>
export default {
  name: 'Group',
  props: {
    name: String,
    speed: Number,
    minPrice: Number,
    maxPrice: Number,
    freeOptions: Array,
    link: String
  },
}
</script>

<style scoped>

</style>