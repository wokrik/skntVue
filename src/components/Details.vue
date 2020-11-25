<template>
  <div class="details" data-content="details" data-details_id="2">
    <div class="details__header">
      <h2>Тариф </h2>
    </div>
    <div class="details__info">
      <div class="details__duration">Период оплаты ― </div>
      <div class="details__price"> ₽/мес</div>
      <div class="details__bill-info">
        <div>разовый платеж ―  ₽</div>
        <div>со счета спишется ―  ₽</div>
      </div>
      <div class="details__dates">
        <div class="details__start-date">вступит в силу ― сегодня</div>
        <span>активно до ― 16.01.2016</span>
      </div>
    </div>
    <div class="details__select-btn btn">Выбрать</div>
  </div>
</template>

<script>
export default {
  name: "Details",
  props: {
    index: Number
  },
  methods: {}
}
</script>

<style scoped>
.details {
  padding-left: 15px;
  margin-bottom: 25px;
  background: white;
  border-top: 1px solid #bfbfbf;
  border-bottom: 1px solid #bfbfbf;
  width: 100%;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}

.details__header {
  color: #6fb316;
  padding: 20px 0;
}

.details__info {
  border: 1px solid #cccccc;
  border-right: none;
  border-left: none;
}

.details__duration, .details__price {
  font-size: 24px;
  font-weight: 600;
  margin-top: 20px;
}

.details__price {
  margin: 0;
  margin-bottom: 20px;
}

.details__bill-info, .details__dates {
  font-size: 22px;
  margin-bottom: 10px;
}

.details__select-btn {
  padding: 20px;
  margin: 20px;
  text-align: center;
  color: white;
  background: #6fb316;
  font-size: 24px;
  max-width: 650px;
}
</style>