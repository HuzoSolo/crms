<template>
    <table class="container m-5">
      <thead>
        <tr>
          <th><h1>Kategori</h1></th>
          <th><h1>Ders</h1></th>
          <th><h1>Ünite</h1></th>
          <th><h1>Konu</h1></th>
          <th><h1>Araç</h1></th>
          <th><h1>Düzey</h1></th>
          <th><h1>Sil</h1></th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>{{ course1.name }}</td>
          <td>{{ course1.teacher }}</td>
          <td>{{ course1.id }}</td>
          <td>{{ course1.date }}</td>
          <td>{{ course1.date }}</td>
          <td>{{ course1.date }}</td>
          <td><button class="btn custom"><i class="fa-solid fa-trash-can"></i></button></td>
        </tr>
  
        <tr>
          <td>{{ course2.name }}</td>
          <td>{{ course2.teacher }}</td>
          <td>{{ course2.id }}</td>
          <td>{{ course2.date }}</td>
          <td><button class="btn custom"><i class="fa-solid fa-trash-can"></i></button></td>
        </tr>
      </tbody>
    </table>
  </template>
  
  <script>
  export default {
    data() {
      return {
        course1: {
          name: "FFL",
          teacher: "Mehmet X",
          date: new Date().toLocaleDateString(),
          id: "332-A",
          
        },
        course2: {
          name: "MMA",
          teacher: "Ahmet Y",
          date: new Date().toLocaleDateString(),
          id: "221-CB",
          
        },
      };
    },
  };
  </script>
  
  <style lang="scss" scoped>
  @import "/src/assets/scss/_colors.scss";
  @import url(https://fonts.googleapis.com/css?family=Open+Sans:300,400,700);
  
  body {
    font-family: "Open Sans", sans-serif;
    font-weight: 300;
    line-height: 1.42em;
  }
  
  h1 {
    font-size: 3em;
    font-weight: 300;
    line-height: 1em;
    text-align: center;
    color: #000000;
  }
  
  h2 {
    font-size: 1em;
    font-weight: 300;
    text-align: center;
    display: block;
    line-height: 1em;
    padding-bottom: 2em;
    color: #000000;
  }
  
  h2 a {
    font-weight: 700;
    text-transform: uppercase;
    color: $primary-color;
    text-decoration: none;
  }
  
  .container th h1 {
    font-weight: bold;
    font-size: 1em;
    text-align: left;
    color: whitesmoke;
  }
  
  .container td {
    font-weight: normal;
    font-size: 1em;
    -webkit-box-shadow: 0 2px 2px -2px #0e1119;
    -moz-box-shadow: 0 2px 2px -2px #0e1119;
    box-shadow: 0 2px 2px -2px #0e1119;
  }
  
  .container {
    text-align: left;
    overflow: hidden;
    width: 80%;
    margin: 0 auto;
    display: table;
    padding: 0 0 8em 0;
    border-radius: 15px;
    box-shadow: 0 0 10px 1px rgba(0, 0, 0, 0.418);
  }
  
  .container td,
  .container th {
    padding-bottom: 2%;
    padding-top: 2%;
    padding-left: 2%;
  }
  
  /* Background-color of the odd rows */
  .container tr:nth-child(odd) {
    background-color: white;
  }
  
  /* Background-color of the even rows */
  .container tr:nth-child(even) {
    background-color: whitesmoke;
  }
  
  .container th {
    background-color: $primary-color;
  }
  
  .container td:first-child {
    color: $darker-color;
    font-weight: 600;
  }
  
  .container tr:hover {
    background-color: #464a5238;
    -webkit-box-shadow: 0 6px 6px -6px #0e1119;
    -moz-box-shadow: 0 6px 6px -6px #0e1119;
    box-shadow: 0 6px 6px -6px #0e1119;
  }
  
  .container td:hover {
    background-color: $primary-color-v2;
    color: #e2e2e2;
    font-weight: bold;
  
    box-shadow: $darker-color -1px 1px, $darker-color -2px 2px, $darker-color -3px 3px,
    $darker-color -4px 4px, $darker-color -5px 5px, $darker-color -6px 6px !important;
    transform: translate3d(3px, -3px, 0);
  
    transition-delay: 0s;
    transition-duration: 0.4s;
    transition-property: all;
    transition-timing-function: line;
  }
  
  @media (max-width: 800px) {
    .container td:nth-child(4),
    .container th:nth-child(4) {
      display: none;
    }
  }
  </style>
  