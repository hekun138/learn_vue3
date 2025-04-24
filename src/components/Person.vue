<template>
    <div class="person">
        <h2>姓名：{{ name }}</h2>
        <h2>年龄：{{ age }}</h2>
        <button @click="changeName">修改姓名</button>
        <button @click="changeAge">修改年龄</button>
        <button @click="showTel">查看联系方式</button>
    </div>
</template>


<script lang="ts">
    export default {
        name: 'Person',
        data() {
            return {
                name: '张三',
                age: 18,
                gender: '男'
            }
        },
        methods: {
            showTel() {
                alert('查看联系方式')
            },
            changeName() {
                this.name = '李四'
            },
            changeAge() {
                this.age += 1;
            }
        }
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