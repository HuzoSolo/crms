<template>
  <h3>Grup Ekleme Formu</h3>
  <form id="group-form">
    <label for="course-category">Ders Kategorisi:</label>
    <select id="course-category" name="course-category" required>
      <option value="" disabled selected>Seçiniz</option>
      <option value="1">Robotik</option>
      <option value="2">Resim kursu</option>
    </select>

    <label for="group-level">Grup Düzeyi:</label>
    <select id="group-level" name="group-level" required>
      <option value="" disabled selected>Seçiniz</option>
      <option value="1">ilkokul</option>
      <option value="2">ortaokul</option>
    </select>

    <label for="lesson-name">Ders Adı:</label>
    <select id="lesson-name" name="lesson-name" required>
      <option value="" disabled selected>Seçiniz</option>
      <option value="1">WEDO</option>
      <option value="2">SPIKE PRIME</option>
    </select>

    <label for="classroom">Sınıf:</label>
        <select id="classroom" name="classroom" required>
        <option value="" disabled selected>Seçiniz</option>
        <option value="1">R1</option>
        <option value="2">R2</option>
    </select>


    <label for="group-day">Ders Günü:</label>
        <select id="group-day" name="group-day" required>
        <option value="" disabled selected>Seçiniz</option>
        <option value="1">Pazartesi</option>
        <option value="2">Salı</option>
    </select>

    <label for="group-hour">Ders Saati:</label>
        <select id="group-hour" name="group-hour" required>
        <option value="" disabled selected>Seçiniz</option>
        <option value="1">16.00</option>
        <option value="2">10.00</option>
    </select>


    <label for="group-teacher">Öğretmen:</label>
        <select id="group-teacher" name="group-teacher" required>
        <option value="" disabled selected>Seçiniz</option>
        <option value="1">Öğretmen 1</option>
        <option value="2">Öğretmen 2</option>
    </select>

    <label for="group-assistant">Asistan:</label>
        <select id="group-assistant" name="group-assistant" required>
        <option value="" disabled selected>Seçiniz</option>
        <option value="1">asistan 1</option>
        <option value="2">asistan 2</option>
    </select>


    <button type="submit">Kaydet</button>
  </form>

  <h3 class="mt-5">Öğrenci Grup kayıt Formu</h3>
  <form id="group-student-form">

    <label for="studentid">Öğrenci ID:</label>
    <input type="number" id="studentid" name="studentid" required />

    <label for="groupid">Grup ID:</label>
    <input type="number" id="groupid" name="groupid" required />

    
    <button type="submit">Kaydet</button>
  </form>


</template>
  
  <script>
export default {};
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