<template>
  <div class="row frame">
    <div class="col-6 p-4">
      <h4 class="header text-center">Mevcut Kategoriler</h4>
      <ul class="list-group list-group-flush">
        <li class="list-group-item text-center">Kategori</li>
        <li class="list-group-item text-center">Kategori</li>

      </ul>
    </div>
    <div class="col-6 p-4">
        <h4 class="header">Kategori Ekle</h4>
        <div class="input-group mb-3">
            <input type="text" class="form-control" placeholder="Kategori adı" aria-label="Recipient's username"
            aria-describedby="button-addon2">
            <button class="btn btn-outline-danger" type="button" id="button-addon2">Ekle</button>
        </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
.frame {
  border-radius: 4px;
  box-shadow: #292929 0px 0px 3px 0px;
}

</style>