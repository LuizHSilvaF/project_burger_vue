<template>
    <div id="nav">
        <router-link to="/" id="logo-url">
            <img :src="logo" :alt="alt" id="logo">
        </router-link>
        <div id="links"> 
            <router-link to="/">Home</router-link>
            <router-link to="/pedidos">Pedidos</router-link>
       </div>
    </div>
</template>

<script>
    export default{
        name: 'Navbar',
        props: ['logo', 'alt']  
    }
</script>

<style scoped>
    #nav{
        background-color: #222;
        border-bottom: 4px solid #111;
        padding: 15px 50px;
        display: flex;
        justify-content: end;
        align-items: center;
    }

    #logo-url{
        margin: auto;
        margin-left: 0;
    }

    #logo{
        width: 40px;
        height: 40px;
    }

    #logo:hover{
        opacity: 60%;
    }
    
    #links a{
        color: #fcba03;
        text-decoration: none;
        margin: 15px;
        transition: .5s;
    }

    #links a:hover{
        color: white;
    }
</style>
