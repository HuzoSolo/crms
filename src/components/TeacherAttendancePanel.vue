<template>
    <div class="attendance-panel">
      <h1>Yoklama Paneli</h1>
  
      <div class="form-group">
        <label for="class">Sınıf:</label> <br>
        <select id="class" v-model="selectedClass" class="select-input">
          <option value="">Sınıf Seçin</option>
          <option v-for="classItem in classes" :key="classItem" :value="classItem">{{ classItem }}</option>
        </select>
      </div>
  
      <div class="form-group">
        <label for="group">Grup:</label><br>
        <select id="group" v-model="selectedGroup" class="select-input">
          <option value="">Grup Seçin</option>
          <option v-for="groupItem in groups" :key="groupItem" :value="groupItem">{{ groupItem }}</option>
        </select>
      </div>
  
      <div class="form-group">
        <label for="subject">Konu:</label><br>
        <input id="subject" type="text" v-model="selectedSubject" class="text-input" />
      </div>
  
      <div class="form-group">
        <label for="date">Tarih:</label><br>
        <input id="date" type="date" v-model="selectedDate" class="date-input" />
      </div>
  
      <br><button @click="takeAttendance" class="submit-button">Yoklamayı Kaydet</button>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        selectedClass: '',
        selectedGroup: '',
        selectedSubject: '',
        selectedDate: ''
      };
    },
    computed: {
      classes() {
        // Sınıf listesini burada doldurun
        return ['9A', '9B', '10A', '10B'];
      },
      groups() {
        // Grup listesini burada doldurun
        return ['A', 'B', 'C', 'D'];
      }
    },
    methods: {
      takeAttendance() {
        if (this.selectedClass && this.selectedGroup && this.selectedSubject && this.selectedDate) {
          // Seçimlerinizi burada kullanarak yoklamayı kaydedin veya başka bir işlem yapın
          console.log('Yoklama kaydedildi!');
          console.log('Sınıf:', this.selectedClass);
          console.log('Grup:', this.selectedGroup);
          console.log('Konu:', this.selectedSubject);
          console.log('Tarih:', this.selectedDate);
        } else {
          alert('Lütfen tüm alanları doldurun!');
        }
      }
    }
  };
  </script>

  <style lang="scss">
$primary-color:#c13832;
$primary-color-v2:#c23129;

  $primary-color: #c13832;
  $secondary-color: #c23129;
  $background-color: #f4f4f4;
  $border-radius: 4px;
  
  .attendance-panel {
    display: flex;
    flex-direction: column;
    align-items: center;
    padding: 20px;
    background-color: $background-color;
  }
  
  h1 {
    margin-bottom: 20px;
    color: $primary-color;
  }
  
  .form-group {
    margin-bottom: 20px;
  }
  
  label {
    display: block;
    margin-bottom: 5px;
    color: $primary-color;
  }
  
  .select-input,
  .text-input,
  .date-input {
    width: 300px;
    padding: 10px;
    border: 1px solid $secondary-color;
    border-radius: $border-radius;
  }
  
  .submit-button {
    padding: 10px 20px;
    background-color: $primary-color;
    color: white;
    border: none;
    border-radius: $border-radius;
    cursor: pointer;
    transition: background-color 0.3s;
  
    &:hover {
      background-color: darken($primary-color, 10%);
    }
  }
  </style>
  