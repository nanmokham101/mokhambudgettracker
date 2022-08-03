<template>
  <header>
    <h1>Budget Tracker</h1>
    <div class="total-income">{{ totalIncome }} MMK</div>
  </header>
</template>

<script>
import Header from '@/components/Header.vue';
export default {
  props: {
    totalIncome: Number
  },
  components:{Header}
}
</script>

<style scoped>
header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 15px 30px;
  background-color: #7c409A;
  border-bottom: 5px solid #000;
}
header h1 {
  color: #EEE;
  font-size: 28px;
}
header .total-income {
  font-family: 'Fira Code', 'Fira Sans', sans-serif;
  background-color: #000;
  color: #FFF;
  font-size: 20px;
  font-weight: 900;
  padding: 5px 10px;
  min-width: 100px;
  text-align: center;
  border-radius: 8px;
  box-shadow: inset 0px 0px 6px rgba(0, 0, 0, 0.25);
  text-shadow: 0px 3px 3px rgba(0, 0, 0, 0.25);
}
</style>