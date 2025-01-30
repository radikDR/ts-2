<script setup lang="ts">
import Cart from './components/Cart.vue';
/*
Задание:
  1. Описать все сущности и функции при помощи интерфейсов и типов Typescript
  2. Реализовать удаление товара, изменение количества и вывод итоговой суммы всей корзины
  3. Цены приведены в копейках, выводить нужно в рублях
*/
</script>

<template>
  <div>
    <h1>Магазин электроники</h1>
    <div class="head">
      <div class="sum">
        <span class="sum-title">Всего:</span>
        <span class="sum-value">1000</span>
      </div>
    </div>

    <Cart />

    <button class="checkout" @click="submit">Посчитать</button>
  </div>
</template>
