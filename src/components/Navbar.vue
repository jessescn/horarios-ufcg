<template>
    <div class="navbar">
        <div id="curso">{{curso}}</div>
        <h1>Horários UFCG</h1>
        <span id="icon-search"><i class="fas fa-search"></i></span>
    </div>
</template>

<script>
export default {
    name: "navbar",
    data() {
        return {
            curso: "Ciência da Computação"
        }
    }
}
</script>

<style>
    div.navbar {
        -webkit-box-shadow: 1px 3px 6px 0px rgba(56, 50, 50, 0.42);
        -moz-box-shadow:    1px 3px 6px 0px rgba(56, 50, 50, 0.42);
        box-shadow:         1px 3px 6px 0px rgba(56, 50, 50, 0.42); 
        position: fixed;
        top: 0;
        width: 100%;
        display: grid;
        grid-template-columns: repeat(3, 1fr);
        justify-content: space-between;
        background-color: #521782;
        color: #E8E8E8; 
        font-family: 'Montserrat', sans-serif;
    }
    
    div.navbar > h1 {
        margin: 0;
        padding: 0;
        font-weight: lighter;
        align-self: center;
        text-align: center;
    }

    #curso {
        background-color: #421268;
        font-size: 20px;
        padding: 13px;
        justify-self: start;
        font-weight: lighter;
    }

    #icon-search {
        display: flex;
        justify-items: center;
        align-items: center;
        font-size: 24px;
        padding: 0 16px;
        justify-self: flex-end;
    }

    @media screen and (max-width: 900px) {
        #curso {
              font-size: 15px;
              padding: 13px;
        }

        div.navbar > h1 {
            font-size: 25px;
        }
    }

    @font-face {
        font-family: Montserrat;
        src: url('../assets/Montserrat-SemiBold.ttf');
    }
</style>

