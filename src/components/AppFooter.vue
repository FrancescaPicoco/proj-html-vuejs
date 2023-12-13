<script></script>

<template>
    <div class="footerWrapper">
        <div class="one">
            <p>CONTACT INFO</p>
            <div class="d-flex">
                <div class="img">
                    <img src="../../public/img/footer-location-dot-solid.svg">
                </div>
                <div>
                    <span>2/45 Tower Street, New York USA</span>
                </div>
            </div>
            <div class="d-flex">
                <div class="img">
                    <img src="../../public/img/footer-phone-solid.svg">
                </div>
                <div>
                    <span>Call Us 0800840 On 1010</span>
                </div>
            </div>
            <div class="d-flex">
                <div class="img">
                    <img src="../../public/img/footer-envelope-soli.svg">
                </div>
                <div>
                    <span>Demo@Example.com</span>
                </div>
            </div>
        </div>
        <div class="two">
            <p>INFORMATION</p>
            <span>Product Support</span>
            <span>Checkout</span>
            <span>Report Abuse</span>
            <span>Redeem Voucher</span>
            <span>Orde Status</span>
        </div>
        <div class="three">
            <p>USEFUL LINKS</p>
            <span>Policies & Rules</span>
            <span>Privacy Policy</span>
            <span>License Policy</span>
            <span>My Account</span>
            <span>Locality</span>
        </div>
        <div class="four">
            <p>NEWS</p>
            <span>Subscribe To Receive Inspiration,</span>
            <span>Ideas & News In Your Inbox.</span>
            <input type="email" placeholder="Enter Your Email" id="mailInput">
            <button>SUBSCRIBE</button>
        </div>
    </div>
    <div class="bgFoot">
        <hr>
        <span class="copy"> &copy; All Rights Reserved. Developed By TemplateMela</span>
    </div>
</template>

<style  lang="scss" scoped>
  @use '../styles/partials/_variables.scss' as *;
.footerWrapper{
    display: flex;
    background-color: $darkTheme;
    color: white;
    justify-content: space-around;
    line-height: 2;
}
.bgFoot{
    background-color: $darkTheme;
    padding: 2rem;
}
.one , .two , .three , .four{
    display: flex;
    flex-direction: column;
    padding: 3rem;
}
p{
    font-size: 20px;
}
.copy{
    display: flex;
    justify-content: center;
    align-items: center;
    margin-top: 50px;
}
img{
    width: 100%;
}
.img{
    width: 15px;
    height: 15px;
}
.d-flex{
    display: flex;
}
span{
    font-size: 19px;
    color: rgb(153, 168, 183);
}
button{
    background-color: white;
    border-radius: 0;
    margin-top: 1rem;
    
}
#mailInput{
    padding: 1rem 2rem;
    background-color: #1c1c1c;
    border: none;
    margin: 0.3rem;
}
</style>