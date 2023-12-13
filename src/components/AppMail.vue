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
            <div>
                <button>SUBMIT</button>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
 @use '../styles/partials/_variables.scss' as *;
span{
    line-height: 1.5;
}
.mailWrapper , .top , .bottom{
    display: flex;
}
.mailWrapper{
    padding: 1rem;
    margin-left: auto;
    margin-right: auto;
    justify-content: center;
}
.right , .left{
    width: 50%;
    text-align: left;
    margin: 1.5rem;
}
.left{
    flex-direction: column;
}
input{
    padding: 0.5rem 2rem 0.5rem 0.5rem ;
    margin: 1rem;
    background-color: rgb(223, 223, 223);
    border: none;
    font-size: 18px;
}
.textMsg{
    padding-bottom: 10rem;
    padding-right: 20rem;
}
button{
    background-color: $darkTheme;
    color: white;
    padding: 1rem 15rem;
    margin-left: 20px;
    border-radius: 0;
}
</style>