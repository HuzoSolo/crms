<template>
  <h3>Öğrenci Kayıt Formu</h3>
  <form id="student-form">
    
    <label for="name">Ad:</label>
    <input type="text" id="name" name="name" required>
        
    <label for="surname">Soyad:</label>
    <input type="text" id="surname" name="surname" required>

    <label for="email">E-mail:</label>
    <input type="text" id="email" name="email">

    <label for="telephone">Telefon no:</label>
    <input type="tel" id="telephone" name="telephone" required>

    <label for="birthdate">Doğum Tarihi:</label>
    <input type="date" id="birthdate" name="birthdate" required> 

    
   <label for="schoolName">Okul adı:</label>
    <input type="text" id="schoolName" name="schoolName" required>

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


    <label for="address">Adres:</label>
    <input type="text" id="address" name="address" required>

    <label for="city">Şehir:</label>
    <select id="city" name="city" required>
      <option value="" disabled selected>Seçiniz</option>
      <option value="1">istanbul</option>
      <option value="2">Ankara</option>
    </select>

    <label for="county">ilçe:</label>
    <select id="county" name="county" required>
      <option value="" disabled selected>Seçiniz</option>
      <option value="1">Çankaya</option>
      <option value="2">Mamak</option>
    </select>

    <label for="discount">iskonto:</label>
    <input type="number" id="discount" name="discount" required>

    <label for="shirt-size">T-shirt Bedeni:</label>
    <select id="shirt-size" name="shirt-size" required>
      <option value="" disabled selected>Seçiniz</option>
      <option value="1">S</option>
      <option value="2">M</option>
      <option value="3">L</option>
    </select>


    <label for="parent-name">Veli Adı:</label>
    <input type="text" id="parent-name" name="parent-name" required>

    <label for="parent-surname">Veli Soyadı:</label> 
    <input type="text" id="parent-surname" name="parent-surname" required>

    <label for="parent-email">Veli E-mail:</label>
    <input type="text" id="parent-email" name="parent-email" required>

    <label for="parent-telephone">Veli Telefon no:</label>
    <input type="tel" id="parent-telephone" name="parent-telephone" required>

    <label for="parent-address">Veli Adres:</label>
    <input type="text" id="parent-address" name="parent-address" required>

    <label for="parent-city">Veli Şehir:</label>
    <select id="parent-city" name="parent-city" required>
      <option value="" disabled selected>Seçiniz</option>
      <option value="1">istanbul</option>
      <option value="2">Ankara</option>
    </select>

    <label for="parent-county">Veli ilçe:</label>
    <select id="parent-county" name="parent-county" required>
      <option value="" disabled selected>Seçiniz</option>
      <option value="1">Çankaya</option>
      <option value="2">Mamak</option>
    </select>

    <label for="parent-job">Veli Meslek:</label>
    <input type="text" id="parent-job" name="parent-job" required>

    


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