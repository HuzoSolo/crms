<template>
    <h3>Kurs Kayıt Formu</h3>
    <form id="course-form">
      <label for="name">Kurs Adı:</label>
      <input type="text" id="name" name="name" required>
  
      <label for="description">Kurs Açıklaması:</label>
      <input type="text" id="description" name="description" required>
  
      <label for="course-day">Kurs Günü:</label>
      <select id="course-day" name="course-day" required>
        <option value="" disabled selected>Kurs Günü</option>
        <option value="1">Pazartesi</option>
        <option value="2">Salı</option>
        <option value="3">Çarşamba</option>
        <option value="4">Perşembe</option>
        <option value="5">Cuma</option>
        <option value="6">Cumartesi</option>
        <option value="7">Pazar</option>
      </select>
  
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