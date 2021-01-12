<template>
  <main id="about" class="about"> 
    <Header/>
    <!-- {{ $t('aboutHeaderTitle') }}  -->
    <div class="container is-fluid about-hero">
        <div class="columns about-intro">
            <div class="column is-6 has-text-left">
                <img src="@/assets/img/about-kuppa.jpg?auto=compress,format"/>
            </div> 
            <div class="column is-4 has-text-left about-content">
                <h1>Kuppa Dropshipping App Romania</h1>
                <p><strong>Dropshipping is a business model. You find the right stuff to sell, then find the right customers to buy it.</strong></p>
                <p>Test out new products and prices without splashing cash upfront. No big-cost bulk buy. No box stacking in your living room. No rolls of sticky tape and shipping labels. Dropshipping is totally digital.</p>
                <p>You build your online store, and do the selling. Your suppliers sort the inventory, and ship orders directly to your shoppers.</p>
                <p>There’s no paying suppliers until your customers pay you. That’s the sweet spot. You buy at one price and sell at another. The profit in between? All yours.</p>
            </div>                 
        </div>
    </div>
    <div class="container aboutquote">
        <p>Thomas J. Watson</p>
        <h4><div><p>"Would you like me to give you a formula for success? It's quite simple, really: Double your rate of failure. You are thinking of failure as the enemy of success. But it isn't at all. You can be discouraged by failure or you can learn from it, so go ahead and make mistakes. Make all you can. Because remember that's where you will find success."</p></div></h4>      
    </div>    
    <div class="container aboutlinks">
        <div class="columns is-multiline">
            <div class="column is-6"><a href=""><div class="has-text-center"><h4>Blog &amp; Press</h4></div></a></div>
            <div class="column is-6"><a href=""><div class="has-text-center"><h4>Contact Us</h4></div></a></div>
            <div class="column is-6"><a href=""><div class="has-text-center"><h4>Pentru Furnizori</h4></div></a></div>
            <div class="column is-6"><a href=""><div class="has-text-center"><h4>Pentru Selleri</h4></div></a></div>
        </div>        
    </div> 
    <div class="container is-fluid header-intro aboutlast">
        <div class="container">
            <div class="aboutlast-content"><div class="has-text-center"><p>Everyone must work, but for many of us that job isn’t just a paycheck, it’s an opportunity to express ourselves and make something better. Entrepreneurs and go-getters often feel as if they carry the weight of an entire organization on their backs, and therefore could always use a little extra motivation.</p><a href=""> Become a Kuppa seller </a></div></div>
        </div>
    </div>       
    <Footer/>
  </main>
</template>
<script>

import Header from '@/components/Header.vue'
import Footer from '@/components/Footer.vue'
export default {
  name: 'About',
  components: {
    Header,
    Footer
  }
}
</script>
<style lang="scss">
    #about {
        .about-hero {
            padding:0;
        }
        .about-intro {
            margin:2rem 0;
            align-items: center;
            .column {
                padding:0;
            }
            h1 {
                font-weight:800;
                font-size:2rem;
                line-height: 1;
                color:#1d1d1f;
                margin-bottom:2rem;
            }
            p {
                margin-bottom: 1rem;
            }
            .about-content {
                margin-left:4rem;
            }
        }
        .aboutlinks {
            margin:5rem auto;
            a {
                border-radius: 10px;
                display: flex;
                background: #fbf7ed;
                width: 100%;
                height: 100%;
                padding: 3rem 0;
                align-items: center;
                justify-content: center;
                transition: 0.7s;
                &:hover {
                    background:#fdeab9;
                    h4 {
                        // color:white;
                    }
                }
            }
            h4 {
                font-size:1.5rem;
                color:#1d1d1f;
                line-height: 1;
                font-weight: 600;
            }
        }
        .aboutquote {
            margin: 10rem auto;
            h4 {
                p {
                    color: black;
                    text-align: left;
                    font-size: 2.5rem;
                    font-weight: 500;
                    line-height: 1.5;
                }
            }
            p {
                margin-bottom: 1rem;
                text-align: left;
                font-weight: 800;
                font-size: 1.5rem;
                color: #1d1d1f;
            }
        }
        .aboutlast {
            margin-top:10rem;
            p {
                font-size:1.5rem;
                color:#1d1d1f;
                margin-bottom: 3rem;
            }
            a {
                color: white;
                letter-spacing: 0.2px;
                font-size: 1.1rem;
                text-transform: uppercase;
                font-weight: 700;
                background: #00a98e;
                padding: 1rem 1.5rem 0.8rem;
                border: 2px solid #00a98e;
                transition: 0.7s;
                border-radius: 20px;
                &:hover {
                    background: transparent;
                    color: #00a98e;
                }
            }
        }
    }
</style>

