<template>
<div class="Likes">
            <button @click="count++">
                🤍  {{ count }}
            </button>
        </div>
</template>
<script>
export default{
    name:'LikeButton',
    data(){
        return{
            count: 0
        }
    }
} 

</script>
<style scoped>
.Likes {
    margin: 0;
    text-align: start;
}
button{
    width: 5em;
    height: 3em;
    background-color: red;
    border: none;
    border-radius: 20px;
    color: white;
    font-size: 15px;
    font-weight: bolder;
    padding: 0;
    margin: 0 5px;
}
</style>