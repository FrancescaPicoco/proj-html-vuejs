<script></script>

<template>
    <div class="mailWrapper">
        <div class="left">
            <span>COLLABORATE</span>
            <h1>WANT TO WORK WITH US? LEAVE US A MESSAGE!</h1>
            <span>Lorem ipsum dolor sit amet consectetur adipisicing elit. Aliquid pariatur enim assumenda ducimus minima. Reiciendis quatur at error, rerum perferendis explicabo ipsa! Corporis excepturi explicabo assumenda totam autem laudantium architecto tenetur cumque, magnam eveniet asperiores consequuntur.</span>
        </div>
        <div class="right">
            <div class="top">
                <input type="text" placeholder="Your Name">
                <input type="email" placeholder="Your Email">
            </div>
            <div class="bottom">
                <input type="text" placeholder="Mobile number">
                <input type="text" placeholder="Your Pincode">
            </div>
            <div >
                <input class="textMsg" type="text" placeholder="Enter Your Message">
            </div>
        </div>
    </div>
</template>

<style scoped>
span{
    line-height: 1.5;
}
.mailWrapper , .top , .bottom{
    display: flex;
}
.mailWrapper{
    width: 70%;
    margin-left: auto;
    margin-right: auto;
}
.right , .left{
    width: 40%;
    text-align: left;
    margin: 1.5rem;
}
.left{
    flex-direction: column;
}
input{
    padding: 0.5rem;
    margin: 1rem;
    background-color: rgb(158, 178, 198);
    border: none;
}
.textMsg{
    padding-bottom: 10rem;
    padding-right: 14rem;
}
</style>