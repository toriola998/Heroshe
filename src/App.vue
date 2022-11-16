<template>
    <div>
        <nav class="flex nav-bar">
            <div class="flex">
                <router-link>
                    <img src="@/assets/logomark-primary.svg" 
                         alt="Home-heroshe"
                         height="18"
                         width="127" /> 
                </router-link>
                <p class="help">Help</p>
            </div>
            <button>Menu</button>
        </nav>
        <header>
            <div class="flex">
                <div class="green-bg">
                    <h1>Hi, How can we help?</h1>
                    <input type="search" placeholder="Find answers to questions about heroshe" />
                </div>
            </div>
        </header>  
        <main>
            <section class="get-started">
                <img src="@/assets/logo.png" 
                    alt="Home-heroshe"
                    height=""
                    width="" /> 
                <h2>New to heroshe ? <br> Let's get you started</h2>
                <p>Some basic to get you started with shipping packages form Us to Nigeria.</p>
                <button>Get me started</button>
            </section>

            <section>
                <HerosheCard 
                    cardIcon="@/assets/logo.png" 
                    cardHeading="FAQ" 
                    cardNote="Some basic to get you started with shipping packages form Us to Nigeria." />
            </section>
        </main>  
    </div>  
</template>

<script>
 import HerosheCard from './components/HerosheCard.vue'

export default {
  name: 'App',
  components: {
     HerosheCard
  }
}
</script>

<style> 
    * {
        margin: 0;
        padding: 0;
        box-sizing: border-box;
    }

    .flex {
        display: flex;
        align-items: center;
    }

    .nav-bar {
        justify-content: space-between;
        padding: 1rem;
    }

    button {
        outline: 0;
        border: none;
    }

    .help {
        font-size: 1.3rem;
        font-weight: bold;
        margin-left: .5rem;
    }

    header > div{
       height: inherit;
       justify-content: center;
    }

    header {
        background-color: #024052;
        height: 200px;
        justify-content: center;
    }

    .green-bg h1 {
        color: white;
        padding-bottom: 1rem;
        text-align: center;
    }

    header input {
        padding: 0 5rem;
        height: 2.5rem;
        
    }

    /****Main */
    main {
        padding: 4rem 1.5rem;
    }

    .get-started {
        background-color: #f5f5f5;
        border-radius: 10px;
        padding: 1.5rem;
    }

    .get-started h2 {
        font-size: 2.2rem;
    }

    .get-started p {
        margin: 1.5rem 0;
        line-height: 1.7;
    }

    .get-started h2, .get-started p {
        text-align: center;
    }

    .get-started button,
    .get-started img {
         margin: auto;
         display: block;
    }

    .get-started button {
        color: black;
        background-color: #f1c34e;
        padding: .5rem 1.5rem; 
    }

</style>
