<template>
    <div class="wrapp">
        <div class="wrappleft">

            <div class="MiniImg" />
            <div class="wrapdate">
                <h3>Name</h3>
                <div class="date">
                    <p>{{currentDate()}}</p>
                    
                </div>
            </div>

        </div>

        <p class="dots">⋮</p>
    </div>
</template>
<script>
export default{
    name: 'Namep',
    methods: {
        currentDate() { 
            // var time = setTimeout(()=>{ 
            //     new Date().toLocaleTimeString()
            // }, 500)

            return (
                (new Date().toLocaleDateString())
            + 
            ' || ' 
            + 
            // time
            (new Date().toLocaleTimeString())   
            // setTimeout(()=>{new Date().toLocaleTimeString()}, 1000)
            ) 
        }
        }   
}
</script>
<style scooped>
*{
    margin: 0;
    padding: 0;
}

h3{
    font-size: 15px;
    
}
.wrapp{
    display: grid;
    grid-template-columns: 70% 30%;
}
.wrappleft{
    display: grid;
    grid-template-columns: 70px auto ;
    text-align: start;
}
.wrappleft p{
    font-size: 12px;
    margin: 3px 0;
}
.MiniImg{
    background-image: url('https://ae01.alicdn.com/kf/Hd5d842e9125b492c91b3170e9f9c5e0bA/MPK-Store-Cat-Toy-Cat-Costume-Clip-Tie-for-Cats-and-Dogs-Cat-Collar.jpg_Q90.jpg_.webp');
    background-color: aquamarine;
    background-size: cover;
    background-position: center;
    border-radius: 5px;
    height: 50px;
    width: 50px;
    margin: 0  0.5em ;
}
.dots{
    font-weight: bold;
    font-size: 2.5em;
    margin: 0;
    padding-right: 0.5em;
    text-align: end;
    cursor: pointer;
    color: rgb(97, 103, 103);
}
.date p{
    font-style: oblique;
    font-size: 10px;
}

</style>