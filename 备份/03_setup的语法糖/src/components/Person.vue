<template>
    <div class="person">
        <h2>姓名：{{ name }}</h2>
        <h2>年龄：{{ age }}</h2>
        <button @click="changeName">修改姓名</button>
        <button @click="changeAge">修改年龄</button>
        <button @click="showTel">查看联系方式</button>
    </div>
</template>


<script setup lang="ts" name="Person123">
import { ref } from 'vue';
console.log(this); // undefined
// 数据
const name = ref('张三')
const age = ref(18)
const gender = ref('男')


// 方法
function changeName() {
    name.value = '李四'
}
function changeAge() {
    age.value += 1
}
function showTel() {
    alert('查看联系方式')
}
</script>

<style scoped>
.person {
    background-color: skyblue;
    padding: 20px;
    border-radius: 10px;
}

button {
    margin-right: 10px;
}
</style>