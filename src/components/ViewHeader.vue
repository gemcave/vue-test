<template>
  <div class="hello">
   <h2 class="first-header">{{ msg }}</h2>
   <div class="main-block">
      <div class="single-user" v-for="item in items" :key="item.id">My name is {{item.name}},
and my age {{item.age}} years old.</div>
   </div>
 </div>
</template>

<script>
export default {
  name: 'ViewHeader',
  data() {
    return {
      items: [
        { id: 0, name: 'John', age: 21 },
        { id: 1, name: 'Levi', age: 19 },
        { id: 2, name: 'Tom', age: 15 },
        { id: 3, name: 'Sara', age: 24 },
      ],
    };
  },
  props: {
    msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="less">
 .first-header {
    text-align: center;
    color: rgba(64, 223, 255, 0.881);
 }

 .main-block {
   border: 1px solid  rgba(64, 223, 255, 0.881);
   border-radius: 20px;
   margin: 0 auto;
   max-width: 250px;
   padding: 20px
 }
 .single-user {
   font-weight: 600;
 }
</style>
