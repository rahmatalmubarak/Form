<template>
<div class="customer-form">
<form>
  <div class="form-group">
    <label for="name">Nama Lengkap</label>
    <input type="text" class="form-control" id="name" placeholder="Masukkan Nama Lengkap">
  </div>
  <div class="form-group">
    <label for="email">Alamat Email</label>
    <input type="email" class="form-control" id="email" placeholder="Masukkan email">
  </div>
  <div class="form-group">
    <label for="address">Alamat</label>
    <input type="textarea" class="form-control" id="address" placeholder="Masukkan Alamat">
  </div>
  <button type="submit" class="btn btn-primary">Tambahkan</button>
</form>
</div>
</template>

<script>
export default {
    name: 'customer-form',
}
</script>