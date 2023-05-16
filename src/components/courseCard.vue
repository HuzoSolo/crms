<template>
  <div class="card" @click="active">
    <div v-if="!clicked" class="page1">
      <div class="cardimg">
        <img
          src="https://img.freepik.com/free-vector/blue-purple-floral-pattern_1017-5170.jpg?w=826&t=st=1680006376~exp=1680006976~hmac=12cdaef90e8fdf4dea6d81af3a5c53a251f8265e91648ee3d3fa599ea9cdaa29"
          alt=""
        />
      </div>
      <div class="cardHeader mt-3">
        <h3>{{ CourseName }}</h3>
      </div>
      <hr />
      <p class="leading">{{ CourseDescription }}</p>
    </div>
    <div v-if="clicked" class="page2">
      <ul class="list p-5">
        <li class="context" :class="{done:isDone}" v-for="content in contents" :key="content">{{ content }}</li>
      </ul>
    </div>

    <nav aria-label="...">
      <ul class="paginate">
        <li class="item">
          <a class="link" :class="{ active: navigation1 }"></a>
        </li>
        <li class="item">
          <a class="link" :class="{ active: navigation2 }"></a>
        </li>
      </ul>
    </nav>
  </div>
</template>

<script>
export default {
  components: {},
  data() {
    return {
      CourseName: "Kurs Adı",
      CourseDescription: "Kurs Açıklaması",
      contents: ["İçerik 1", "İçerik 2", "İçerik 3", "İçerik 4"],
      clicked: false,
      navigation1: true,
      navigation2: false,
      isDone: false,
    };
  },
  methods: {
    paginate() {
      this.navigation1 = !this.navigation1;
      this.navigation2 = !this.navigation2;
    },

    active() {
      this.clicked = !this.clicked;
      this.paginate();
    },
  },
};
</script>


<style lang="scss" scoped>

@import "/src/assets/scss/_colors.scss";
.card {
  display: flex;
  width: 25%;
  height: 20%;
  background-color: #f5f5f5;
  border-radius: 10px;
  margin: 10px;
  padding: 15px;
  box-shadow: 0 0 10px 1px rgba(0, 0, 0, 0.418);
  cursor: pointer;
  transition: all 1s ease-in-out;
}

.cardimg img {
  display: flex;
  width: 95%;
  height: 100px;
  object-fit: cover;
  border-radius: 10px;
  margin-left: auto;
  margin-right: auto;
}
.card:hover {
  transform: scale(1.1);
  margin: 23px;
}
.cardHeader {
  display: flex;
  justify-content: space-between;
  text-align: center;
}

.context{
  list-style: upper-roman;
  font-size: 20px;
  font-weight: 500;
  margin-bottom: 10px;
  color: $primary-color;
}
.done{
  color: #368020;
}

.paginate{
  display: flex;
  justify-content: start;
  margin-top: 10px;
  margin-bottom: 10px;
  margin-left: 14px;
  list-style: none;

  .link{
    display: flex;
    width: 15px;
    height: 15px;
    border-radius: 50%;
    border-color: $darker-color;
    border-width: 2px;
    border-style: solid;
    background-color: whitesmoke;
    margin-right: 5px;
    cursor: pointer;
    transition: all 1s ease-in-out;
    
    
  }
  
}

.active{
  background-color: $darker-color !important;
  width: 20px !important;
  height: 20px !important;
}

</style>