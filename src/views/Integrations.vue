<template>
  <main id="integrations" class="integrations"> 
    <Header/>
        <div class="container is-fluid header-intro">
            <h2>Integrari</h2>
            <p>Kuppa se poate conecta cu usurinta de mai multe platforme e-commerce. Astfel vei putea folosi platforma favorita pentru a vinde si a promova produsele alese.</p>
        </div>
        <div class="container integrationsoptions">
            <div class="columns">
                <div class="column">
                    <a href="">
                        <img src="@/assets/img/shopify.png?auto=compress,format">
                        <span>Shopify</span>
                    </a>
                </div>
                <div class="column">
                    <a href="">
                        <img src="@/assets/img/magento.png?auto=compress,format">
                        <span>Magento 2</span>
                    </a>
                </div>
                <div class="column">
                    <a href="">
                        <img src="@/assets/img/woocommerce.png?auto=compress,format">
                        <span>WooCommerce</span>
                    </a>
                </div>
                <div class="column">
                    <a href="">
                        <img src="@/assets/img/bigcommerce.png?auto=compress,format">
                        <span>BigCommerce</span>
                    </a>
                </div>
                <div class="column">
                    <a href="">
                        <img src="@/assets/img/wix.svg">
                        <span>Wix</span>
                    </a>
                </div>
                <div class="column">
                    <a href="">
                        <img src="@/assets/img/merchantpro.png?auto=compress,format">
                        <span>MerchantPro</span>
                    </a>
                </div>
            </div>
        </div>
        <div class="container is-fluid integrationscopybg">
            <div class="container integrationscopy">
                <div class="columns">
                    <ul>
                        <li class="column">
                            <img src="@/assets/img/integrations-howto.jpg?auto=compress,format">
                        </li>
                        <li class="column has-text-left">
                            <h3>Easy steps for your dream business</h3>
                            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed malesuada tristique est vitae lobortis. Phasellus tristique purus ut convallis bibendum. Mauris non urna accumsan, laoreet urna eget, varius sapien. Mauris maximus magna ac lacus gravida, sed sollicitudin ex posuere.  Lorem ipsum dolor sit amet, consectetur adipiscing elit. In bibendum aliquam lorem, vel tincidunt massa molestie quis. Vivamus tincidunt justo massa, tincidunt congue est interdum at. </p>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
        <div class="container integrationshowto">
            <h3>Conectare rapida si eficienta</h3>
            <ol class="columns">
                <li class="column has-text-left">
                    <h5>01</h5>
                    <h4>Creaza cont Kuppa</h4>
                    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. In bibendum aliquam lorem, vel tincidunt massa molestie quis. Vivamus tincidunt justo massa, tincidunt congue est interdum at.</p>
                </li>
                <li class="column has-text-left">
                    <h5>02</h5>
                    <h4>Conectare e-commerce</h4>
                    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. In bibendum aliquam lorem, vel tincidunt massa molestie quis. Vivamus tincidunt justo massa, tincidunt congue est interdum at.</p>
                </li>
                <li class="column has-text-left">
                    <h5>03</h5>
                    <h4>Import rapid produse</h4>
                    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. In bibendum aliquam lorem, vel tincidunt massa molestie quis. Vivamus tincidunt justo massa, tincidunt congue est interdum at.</p>
                </li>
            </ol>
            <div class="columns">
                <div class="column integrationscta">
                    <a href="https://app.kuppa.global"> Creeaza Cont Gratuit </a>
                </div>
            </div>
        </div>
    <Footer/>
  </main>
</template>

<script>

import Header from '@/components/Header.vue'
import Footer from '@/components/Footer.vue'
export default {
  name: 'Integrations',
  components: {
    Header,
    Footer
  }
}
</script>

<style lang="scss">
    #integrations {
         .header-intro {
            h2 {
                font-size:3.5rem;
                font-weight:900;
                color:#1d1d1f;
            }
        }
    }
    .integrationsoptions {
        margin:5rem auto;
        h3 {
            color:#1d1d1f;
            font-size:1.3rem;
            font-weight:700;
        }
        img {
            height:30px;
            margin-bottom:1rem;
        }
        a {
            color:#1d1d1f;
            font-weight:900;
            font-size:1.1rem;
            text-transform: uppercase;
            display:flex;
            flex-direction: column;
            align-items: center;
            transition:0.4s;
            &:hover {
                color:#00a98e;
            }
        }        
    }
    .integrationscopybg {
        padding:5rem 0;
        background:#fafafa;
        margin:3rem auto;
        .integrationscopy {
            ul {            
                display:flex;
                align-items: center;    
                h3 {
                    font-weight:800;
                    font-size:1.4rem;
                    color:#1d1d1f;
                    padding-left:3rem;
                    margin-bottom:1rem;
                }        
                p {
                    padding-left:3rem;
                }
            }
        }        
    }
    .integrationshowto {
        margin:7rem auto;
        h3 {
            font-size:3rem;
            font-weight:800;
            text-align: center;
            color:#1d1d1f;
            margin-bottom:3rem;
        }
        h4 {
            font-size:1.3rem;
            font-weight:800;
            color:#1d1d1d;            
        }
        h5 {
            font-size: 4rem;
            font-weight: 800;
            margin-bottom: 0;
            color: #dedcdc;
            line-height: 1;
        }
        ol {
            li {
                padding:0 3rem;
            }
        }
    }
    .integrationscta {
        margin-top: 3rem;
        a {
            color: white;
            letter-spacing: 0.2px;
            font-size: 1.1rem;
            text-transform: uppercase;
            font-weight: 700;
            background: #00a98e;
            border-radius: 20px;
            padding: 10px 20px 8px 20px;
            border: 2px solid #00a98e;
            transition: 0.7s;
            &:hover {
                background:transparent;
                color:#00a98e;
            }
        }
    }
</style>
