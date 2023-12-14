<script>
 const counterElement = document.getElementById('counter');
        const targetValue = 10000;
        const duration = 4000; // 4 seconds
        const interval = 10; // Update every 10 milliseconds

        const increment = (targetValue / (duration / interval));

        let currentValue = 0;

        const updateCounter = () => {
            currentValue += increment;

            if (currentValue >= targetValue) {
                currentValue = targetValue;
                clearInterval(counterInterval);
            }

            counterElement.textContent = Math.round(currentValue);
        };

        const counterInterval = setInterval(updateCounter, interval);
export default {
    name:'AppCounter',
    // data() {
    //     return {
    //         modules: [Autoplay, Navigation]
    //     };
    // },
    // methods: {
    //     count(){
    //       var counter = 0;
    //       setInterval(() => {
    //         counter++
    //         document.getElementById("uno").innerHTML += counter
    //       } , 1000)
    //     }
    // },
    // mounted() {
    //     count()
    // }
}
</script>

<template>
    <div id="counterWrapper">
         <!-- <div>
            <h1 id="uno"></h1>
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
        </div> -->
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
/* h1{
    margin: 0 3rem;
    font-size: 100px;
}
div{
    text-align: center;
} */
body {
            display: flex;
            align-items: center;
            justify-content: center;
            height: 100vh;
            margin: 0;
        }

        #counter {
            font-size: 3em;
            font-family: 'Arial', sans-serif;
        }
</style>