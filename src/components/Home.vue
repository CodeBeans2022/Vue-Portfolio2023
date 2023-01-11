<template>
<div class="background">
    <div class="homeText">
    <h1 class="display-6">Bonjour, I'm Jamie-Lee Kinnear.</h1>
    <h2 class="lead">Aspiring Full-Stack Developer and I.T Engineer.</h2>
</div>
</div>
</template>

<script>
export default {
name: 'Home'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.homeText{
    width: 100% ;
    height: 100%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}

.background{
    width: 100%;
    height: 100vh;
    background-image: url(https://i.postimg.cc/5NvPPhgY/myimage.png);
    background-size: cover;
    background-repeat: no-repeat;
    box-shadow: inset 120px 100px 250px #000000, inset -120px -100px 250px #000000;
}

h1, h2{
    color: white;
    text-align: center;
}
</style>
