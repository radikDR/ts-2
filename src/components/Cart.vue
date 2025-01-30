<template>
    <div class="cart">
      <CartItem v-for="item in products" :key="item.id" :item="item" />
    </div>
  </template>
  
  <script>
  import CartItem from './CartItem.vue';
  
  const data = [
    {
      id: 1,
      title: "Xiaomi Poco C75",
      price: 1130000,
      quantity: 1,
    },
    {
      id: 2,
      title: "Samsung Galaxy S24",
      price: 9000000,
      quantity: 3,
    },
    {
      id: 3,
      title: "REALME C63",
      price: 1600000,
      quantity: 2,
    },
    {
      id: 4,
      title: "Apple iPhone 15",
      price: 8400000,
      quantity: 1,
    },
    { id: 5, title: "Xiaomi Poco C61", price: 650000, quantity: 10 },
  ];
  
  export default {
    name: 'Cart',
    components: {
      CartItem,
    },
    data() {
      return {
        products: data,
      };
    },
    mounted() {
      console.log('child');
    },
  };
  </script>
  
  <style>
  /* Ваши стили */
  </style>