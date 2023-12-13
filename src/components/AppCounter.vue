<script>
export default {
    name:'AppCounter',
}
</script>

<template>
    <div id="counterWrapper">
        <div>
            <h1>780</h1>
            <span>SATISFIED CLIENTS</span>
        </div>
        <div>
            <h1>20+</h1>
            <span>OUR PROJECTS</span>
        </div>
        <div>
            <h1>10,000</h1>
            <span>CUP OF COFFEE</span>
        </div>
        <div>
            <h1>712</h1>
            <span>OUR AWARDS</span>
        </div>
    </div>
</template>

<style scoped>

#counterWrapper{
    height: 30vh;   
    color: white;
    display: flex;
    justify-content: center;
    align-items: center;
    background-image: url("../../public/img/Parallax-01.jpg");
    min-height: 30vh;
    background-attachment: fixed;
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
}
h1{
    margin: 0 3rem;
    font-size: 100px;
}
div{
    text-align: center;
}
</style>