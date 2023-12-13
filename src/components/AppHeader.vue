<script>

</script>

<template>
    <div id="fixhead">
        <div id="headerWrapper">
        <div>
            <img id="logo" src="../../public/img/logo.svg">
        </div>
        <div id="navbar">
            <a href="#">HOME</a>
            <a href="#">BLOG</a>
            <select name="about">
                <option>ABOUT</option>
                <option>Services</option>
                <option>Our work flow</option>
                <option>Video thumbnail type</option>
            </select>
            <a href="#">ABOUT</a>
            <a href="#">CONTACS</a>
            <a href="#">GALLERY</a>
            <select name="shop">
                <option>SHOP</option>
                <option>shop pages</option>
                <option>product type</option>
            </select>
        </div> 
        <div id="cerca">
            <img id="search" src="../../public/img/image (8).svg">
            <img id="icn" src="../../public/img/image (9).svg">
            <img id="icn" src="../../public/img/image (10).svg">
            <img id="icn" src="../../public/img/image (11).svg">
            <img id="icn" src="../../public/img/image (12).svg">
        </div>       
        </div>
    </div>
    
</template>

<style lang="scss" scoped>
  @use '../styles/partials/_variables.scss' as *;
#fixhead{
    position: relative;
}
#headerWrapper{
    width: 100%;
   position: absolute;
   height: 13vh;
   background-color: $whiteTheme;
   display: flex;
   align-items: center;
   justify-content: space-between;
   position: fixed;
   z-index: 999;
}
#logo{
    width: 90%;
   margin-left: 1rem;
}
a {
    margin: 1rem;
    color: black;
    text-decoration: none;
}
option{
    border: none;
}
#cerca{
    display: flex;
    align-items: center;
    padding: 1rem;
}
#search{
    width: 70%;
    border-right: 1px solid black;
    padding-right: 1rem;
}
#icn{
    margin: 0 1rem;
}
</style>   