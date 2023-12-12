<script></script>

<template>
    <div class="aboutUsWrapper">
        <img src="../../public/img/About-Us.jpg">
        <div id="aboutUsAbsolute">
            <div>
                <span>ABOUT US</span>
                <h1>HIGH QUALITY CINEMATICS</h1>
                <span>Lorem ipsum dolor sit amet consectetur adipisicing elit. Atque incidunt at beatae non doloremque id quibusdam? Autem, qui porro fugiat libero distinctio itaque odio facere cum eum perspiciatis eaque explicabo.
                      Officia doloribus dignissimos velit blanditiis repudiandae nesciunt, quasi labore earum exercitationem molestiae deserunt itaque sed, ea architecto, fugit praesentium et placeat optio rem accusantium excepturi dolorum deleniti autem animi? Asperiores.
                </span>
            </div>
            <div>
                <button>READ MORE</button>
            </div>          
        </div>         
    </div>    
</template>

<style scoped>
img{
    width: 100%;
    height: 500px;
}
.aboutUsWrapper{
    position: relative;
}
#aboutUsAbsolute{
    position: absolute;
    top:30px;
    right: 0;
    width: 700px;
    height: 400px;
}
h1{
    margin-top: 0;
}
span , h1{
    color: white;
}
span{
    line-height: 2.5;
}
button{
    background-color: white;
    margin-top: 1.5rem;
}
</style>