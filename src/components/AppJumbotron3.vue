<script></script>

<template>
<div class="positioning">    
    <img src="../../public/img/Parallax-01.jpg">
    <div id="wrapperJumbo">
        <div class="icn">
           <img src="../../public/img/image (20).svg">
        </div>
        <div>
            <span>Lorem ipsum dolor sit amet consectetur adipisicing elit. Nulla officia officiis est possimus. Dignissimos at possimus. Lorem ipsum dolor sit amet consectetur adipisicing elit. Deserunt quo commodi eos aut ratione repellat, consectetur quos libero quod facere ipsum explicabo ab optio repellendus odit similique atque! Est, provident?
            </span>
        </div>
        <div class="profilo">
            <img src="../../public/img/02.jpg">
            <div class="descr">
                <h3>JOHN DOE</h3>
                <span>deigner</span>
            </div>
        </div>
    </div>
</div>
</template>

<style scoped>
#wrapperJumbo{
    width: 60%;
    position: absolute;
    top: 50%;
    left: 20%;
}
.positioning > img{
    width: 100%;
    height: 100%;
}
.positioning{
    position: relative;
    height: 550px;
}
.icn{
    width: 5%;
    filter: invert();
    margin-left: auto;
    margin-right: auto;
}
.profilo{
    display: flex;
    justify-content: center;
    margin-top: 2rem;
}
.desc{
    display: flex;
}
span , h3{
    color: white;
    margin-top: 0;
}

</style>