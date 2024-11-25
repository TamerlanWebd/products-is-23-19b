<script setup>
import { ref } from "vue";
const products = ref([
{
id: Date.now(),
name: "Tesla",
count: 10,
price: 4000,
date: "20.11.2024",
},
{
id: Date.now(),
name: "HP",
count: 15,
price: 5000,
date: "9.10.2024",
},
{
id: Date.now(),
name: "Acer",
count: 5,
price: 10000,
date: "10.06.2024",
},

{
id: Date.now(),
name: "Asus",
count: 20,
price: 8000,
date: "25.11.2024",
},

]);
</script>

<template>
<div class="container">
  <div class="row">

<div class="col">
  <h1 class="text-center my-3">Учет товаров</h1>
  <div class="mb-3">
  <label for="name" class="name">Название</label>
  <input type="text" class="form-control" id="name">
</div>
<div class="mb-3">
  <label for="date" class="date">Дата</label>
  <input type="date" class="form-control" id="date">
</div>
<div class="mb-3">
  <label for="count" class="count">Количество</label>
  <input type="number" class="form-control" id="count">
</div>
<div class="mb-3">
  <label for="price" class="price">Цена</label>
  <input type="number" class="form-control" id="price">
</div>
<button type="button" class="btn btn-outline-primary">Добавить</button>
</div>
<div class="row row-cols-1 row-cols-md-3 g-4">
  <div class="col" v-for="products in products">
    <div class="card h-100">
      <div class="card-body">
        <h5 class="card-title">{{ products.name }}</h5>
        <p class="card-text">${{ products.price }}</p>
        <p class="card-text">x{{ products.count }}</p>
        <p class="card-text">{{ products.date }}</p>
      </div>
      <div class="card-footer text-end">
        <button class="btn btn-outline-danger">Удалить</button>
      </div>
    </div>
  </div>
  
    </div>
<div class="row my-4">
  <div class="col">
    <h3 class="text-end">Общая сумма товаров: $452155</h3>
  </div>
</div>
</div>

</div>
</template>

