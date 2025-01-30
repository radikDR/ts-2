<template>
    <div class="row">
      <div class="title">{{ item.title }}</div>
      <div class="quantity">
        <button class="change">-</button>
        <div class="quantity-value">{{ item.quantity }}</div>
        <button class="change">+</button>
      </div>
      <div class="price">100</div>
      <div class="total">500</div>
      <button class="delete">Удалить</button>
    </div>
  </template>
  
  <script>
  export default {
    name: 'CartItem',
    props: {
      item: {
        type: Object,
        required: true,
      },
    },
  };
  </script>
  
  <style>
  /* Ваши стили */
  </style>