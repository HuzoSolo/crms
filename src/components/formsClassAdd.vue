<template>
  <div class="row frame">
    <div class="col-6 p-4">
      <h4 class="header text-center">Mevcut Dersler</h4>
      <ul class="list-group list-group-flush">
        <li class="list-group-item text-center">
          <span class="text-muted category">Kategori</span>-<span class="fw-800 class">Ders</span>
        </li>
        <li class="list-group-item text-center">
          <span class="text-muted category">Kategori</span>-<span class="fw-800 class">Ders</span>
        </li>
      </ul>
    </div>
    <div class="col-6 p-4">
      <h4 class="header">Ders Ekle</h4>
      <select class="form-select mb-3" aria-label="Default select example">
        <option selected>Kategori Seç</option>
        <option value="1">Kategori 1</option>
        <option value="2">Kategori 2</option>
      </select>
      <div class="input-group mb-3">
        <input
          type="text"
          class="form-control"
          placeholder="Ders Adı"
          aria-label="Recipient's username"
          aria-describedby="button-addon2"
        />
        <button class="btn btn-outline-danger" type="button" id="button-addon2">
          Ekle
        </button>
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