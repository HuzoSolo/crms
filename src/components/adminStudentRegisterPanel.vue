<template>
  <h3>Öğrenci Kayıt Formu</h3>
  <form id="student-form">
    
    <label for="name">Ad:</label>
    <input type="text" id="name" name="name" required>
        
    <label for="surname">Soyad:</label>
    <input type="text" id="surname" name="surname" required>
        
    <label for="address">Adres:</label>
    <input type="text" id="address" name="address" required>

    <label for="birthdate">Doğum Tarihi:</label>
    <input type="date" id="birthdate" name="birthdate" required>

    <label for="class-code">Sınıf Kodu:</label>
    <input type="text" id="class-code" name="class-code" required>

    <label for="class-level">Sınıf Düzeyi:</label>
    <select id="class-level" name="class-level" required>
      <option value="" disabled selected>Seçiniz</option>
      <option value="1">1. Sınıf</option>
      <option value="2">2. Sınıf</option>
      <option value="3">3. Sınıf</option>
      <option value="4">4. Sınıf</option>
      <option value="5">5. Sınıf</option>
      <option value="6">6. Sınıf</option>
    </select>

    <button type="submit">Kaydet</button>
  </form>


</template>

<script>
export default {


    
}
</script>

<style lang="scss" scoped>

$primary-color: #c13832;
$form-width: 400px;

h3 {
  text-align: center;
  color: $primary-color;
}

form {
  max-width: $form-width;
  margin: 0 auto;
  padding: 10px;
  border: 1px solid $primary-color;
  border-radius: 4px;

  label {
    display: block;
    margin-top: 10px;
    color: $primary-color;
  }

  input,
  select {
    width: 100%;
    padding: 5px;
    margin-top: 5px;
    border: 1px solid $primary-color;
    border-radius: 4px;
    box-sizing: border-box;
  }

  button {
    display: block;
    width: 100%;
    padding: 10px;
    margin-top: 10px;
    color: white;
    background-color: $primary-color;
    border: none;
    border-radius: 4px;
    cursor: pointer;
  }

}


</style>