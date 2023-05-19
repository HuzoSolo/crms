<template>

    <h3>Ödeme Ekleme Formu</h3>
    <form id="course-form">
      <label for="studentid">Öğrenci ID:</label>
      <input type="text" id="studentid" name="studentid" required>
        
      <label for="paymentDate">Ödeme Tarihi:</label>
      <input type="date" id="paymentDate" name="paymentDate" required>

      <label for="amount">Miktar:</label>
      <input type="text" id="amount" name="amount" required>
  
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