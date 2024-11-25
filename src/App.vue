<script setup>

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
  </div>
</div>
</template>

