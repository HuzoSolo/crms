<template>
    
    <h3>Eğitmen Kayıt Formu</h3>
    <form id="student-form">
      
      <label for="name">Ad:</label>
      <input type="text" id="name" name="name" required>
          
      <label for="surname">Soyad:</label>
      <input type="text" id="surname" name="surname" required>

      <label for="picture">Resim:</label>
      <input class="form-control" type="file" id="picture" name="picture">

      <label for="gender">Cinsiyet:</label>
        <select id="gender" name="gender" required>
        <option value="" disabled selected>Seçiniz</option>
        <option value="0">Kadın</option>
        <option value="1">Erkek</option>
    </select>

    <label for="marital-status">Medeni Hal:</label>
        <select id="marital-status" name="marital-status" required>
        <option value="" disabled selected>Seçiniz</option>
        <option value="0">Evli</option>
        <option value="1">Bekar</option>
    </select>
  
      <label for="edu-status">Eğitim durumu:</label>
      <input type="text" id="edu-status" name="edu-status" required>

      <label for="uni-name">Üniversite Adı:</label>
      <input type="email" id="uni-name" name="uni-name">

      <label for="birthdate">Doğum Tarihi:</label>
      <input type="date" id="birthdate" name="birthdate" required>
  
      <label for="email">E-posta:</label>
      <input type="email" id="email" name="email" required>

      <label for="phone">Telefon:</label>
      <input type="tel" id="phone" name="phone" required>

      <label for="personal-type">Pozisyon:</label>
      <select id="personal-type" name="personal-type" required>
        <option value="" disabled selected>Seçiniz</option>
        <option value="1">Öğretmen</option>
        <option value="2">Asistan</option>
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