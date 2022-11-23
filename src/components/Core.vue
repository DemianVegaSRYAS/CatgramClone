<template>
<div class="Core">
    <div v-for="image in images" class="Post ">
        <Namep class="Name"/>
        <!-- <div class="Name">Name</div> -->
        <img :src=image.url :key="url" class="Image"/>
        <p class="descrp">Lorem ipsum, dolor sit amet consectetur adipisicing
            elit. Adipisci et architecto sequi nisi, fugiat 
            distinctio illo temporibus rerum officiis, excepturi 
            facere corporis est eum molestiae dolorem laudantium 
            mollitia ullam maiores.</p>
        <div class="Likes">Likes</div>
    </div>
    
</div>
</template>
<script>
import Namep from '@/components/Namep.vue'
export default {
    name: 'Core',
    components:{
        Namep,
    },data(){
        return{
            images:[
                {url:'https://data.whicdn.com/images/357279301/original.jpg'},
                {url:'https://assets-global.website-files.com/61bbcec54a71bb14e2611c3a/61bbcec54a71bb9a1b612216_Can%20cats%20have%20Benadryl_Hero.jpg'},
                {url:' https://www.animalmedical.net/blog/wp-content/uploads/2021/02/iStock-149052633-1-1.jpg'},
                {url:'https://media.istockphoto.com/id/916159418/photo/cute-kitten-portrait-british-shorthair-cat.jpg?s=612x612&w=0&k=20&c=Fxeq0syWLxQ_iZgxe2rSy-1l-tQxtDVGkE-0N02gF98='},
                {url:'https://preview.redd.it/bci4lmss17881.jpg?width=3024&format=pjpg&auto=webp&s=a9f8d1740418ac7e230953168bd2a28a34a168c3'},
                {url:'https://external-preview.redd.it/EuV0onSY_Pz3O0ZJFkGqGOG5aqFv5EOTn-ZgA5iUQRw.jpg?width=640&crop=smart&auto=webp&s=b3faea23414f05c555e5660424ab9e75ea74b40c'},
            ]
        }
    }
}


</script>
<style scooped>
.Core{
    color: white;
    background-color: rgb(0, 0, 0);
    height: 80vh;
    overflow-y: scroll;
}
::-webkit-scrollbar {
    display: none;
}
.Image{
    /* background-image: url('https://data.whicdn.com/images/357279301/original.jpg'); */
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
    padding: 0;
    width: 100%;
    height: 100%;
    margin: 0.5em 0;
}
.Post{
    height: auto;
    background-color: rgba(103, 103, 103, 0.466);
    margin: 1em;
    display: grid;
    grid-template-rows: 50px auto auto 50px;
    border-radius: 10px;
    padding-top: 1em;
    /* overflow-y: scroll; */
}
.Likes {
    margin: 0;
}
p{
    margin: 1em;
}
.descrp{
    text-align: justify;
    font-style: oblique;
}
</style>