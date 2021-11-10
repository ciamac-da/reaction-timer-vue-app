<template>
<div class="block"> Click Me </div>
</template>

<script>
export default {
    name: "Block",
    props:["delay"],
    data() {
    return {
    showBlock: false
     }
    },
    mounted() {
    setTimeOut(()=> {
    this.showBlock = true
    }, this.delay)
    },
}
</script>

<style scoped>
.block {
    width: 400px;
    border-radius: 20px;
    background: green;
    color: white;
    text-align: center;
    padding: 100px 0;
    margin: 40px auto;
}
</style>