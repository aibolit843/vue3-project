<template>
    <div class="navbar">
        <div @click="$router.push('/')">Vue 3</div>
        <div class="navbar__btns">
           <my-button @click="$router.push('/posts')">Посты</my-button>
           <my-button @click="$router.push('/about')" style="margin-left: 20px">О приложении</my-button>
           <my-button @click="$router.push('/store')" style="margin-left: 20px">store</my-button>
           <my-button @click="$router.push('./composition')" style="margin-left: 20px">composition</my-button>
        </div>
    </div>
</template>

<script>
import MyButton from './UI/MyButton.vue'
export default {
  components: { MyButton },
    
}
</script>

<style scoped>
.navbar {
    height: 70px;
    background-color: lightgray;
    box-shadow: 2px 2px 4px grey;
    display: flex;
    align-items: center;
    padding: 0 15px;
}
.navbar__btns {
    padding: 15px;
    margin-left: auto;
    margin-bottom: 10px;
}
</style>