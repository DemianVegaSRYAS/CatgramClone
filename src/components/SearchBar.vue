<template>
    <div class="hello">
        <input type="text" placeholder=" Search Cats...">
        <!-- 🔎 -->
    </div>
</template>
<script>
export default{
    name:'SearchBar',
}
</script>
<style scooped>
input{
    width: 400px;
    background-color: rgba(141, 139, 139, 0.304) ;
    background-image: url('https://upload.wikimedia.org/wikipedia/commons/thumb/d/de/OOjs_UI_icon_search-ltr.svg/480px-OOjs_UI_icon_search-ltr.svg.png');
    background-size: 20px;
    background-position: start;
    background-position-y: center;
    background-repeat: no-repeat;
    background-position-x: 10px;
    border-radius: 20px;
    font-size: 1em;
    padding: 0.5em 1em;
    padding-left: 2.5em;
    color: rgb(255, 255, 255);
    filter: invert(30%);

    border-color: transparent;
}
input:focus-visible {
    outline-width: 0;
    }
</style>