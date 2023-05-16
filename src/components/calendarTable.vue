<template>
    <div class="calendar">
      <div class="calendar-header">
        <button class="btn custom" @click="previousMonth">&lt;</button>
        <h2>{{ month }} {{ year }}</h2>
        <button class="btn custom" @click="nextMonth">&gt;</button>
      </div>
      <div class="calendar-grid">
        <div v-for="day in daysOfWeek" :key="day" class="calendar-cell day">{{ day }}</div>
        <div v-for="date in dates" :key="date" :class="['calendar-cell', { today: isToday(date) }]" @click="selectDate(date)">{{ date }}</div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'CalendarTable',
    data() {
      return {
        selectedDate: null,
        month: null,
        year: null,
        daysOfWeek: ['Sun', 'Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat'],
        dates: []
      };
    },
    mounted() {
      const today = new Date();
      this.month = today.toLocaleString('default', { month: 'long' });
      this.year = today.getFullYear();
      this.generateDates(today.getMonth(), today.getFullYear());
    },
    methods: {
      previousMonth() {
        const currentMonth = new Date(this.year, this.getMonthNumber(this.month), 1);
        currentMonth.setMonth(currentMonth.getMonth() - 1);
        this.month = currentMonth.toLocaleString('default', { month: 'long' });
        this.year = currentMonth.getFullYear();
        this.generateDates(currentMonth.getMonth(), currentMonth.getFullYear());
      },
      nextMonth() {
        const currentMonth = new Date(this.year, this.getMonthNumber(this.month), 1);
        currentMonth.setMonth(currentMonth.getMonth() + 1);
        this.month = currentMonth.toLocaleString('default', { month: 'long' });
        this.year = currentMonth.getFullYear();
        this.generateDates(currentMonth.getMonth(), currentMonth.getFullYear());
      },
      generateDates(month, year) {
        this.dates = [];
        const daysInMonth = new Date(year, month + 1, 0).getDate();
        for (let i = 1; i <= daysInMonth; i++) {
          this.dates.push(i);
        }
      },
      getMonthNumber(monthName) {
        const date = new Date(Date.parse(`${monthName} 1, 2022`));
        return date.getMonth();
      },
      isToday(date) {
        const today = new Date();
        return this.year === today.getFullYear() && this.getMonthNumber(this.month) === today.getMonth() && date === today.getDate();
      },
      selectDate(date) {
        this.selectedDate = new Date(this.year, this.getMonthNumber(this.month), date);
        this.$emit('date-selected', this.selectedDate);
      }
    }
  };
  </script>
  
  <style>
    .calendar {
        margin-bottom: 10%;
        margin-left: auto;
        margin-right: auto;
        width: 50% !important;
        box-shadow: 0 0 10px 0 rgba(0, 0, 0, 0.2);
        border-radius: 15px;
        padding: 20px;

    }

  .calendar-header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 10px;
    padding-bottom: 20px;
    border-bottom: rgba(0, 0, 0, 0.274) 1px solid;
  }
  
  .calendar-grid {
    display: grid;
    grid-template-columns: repeat(7, 1fr);
    grid-template-rows: repeat(5, 1fr);
    grid-gap: 16px;
  }
  
  .calendar-cell {
    display: flex;
    justify-content: center;
    align-items: center;
    background-color: #fff;
    /* border: 1px solid #ddd; */
    font-size: 16px;
    font-weight: 700;
    width: 100px;
    height: 100px;
  }
  
  .today {
    background-color:brown ;
    border-radius: 50%;
    color: #fff;
  }
  </style>
  