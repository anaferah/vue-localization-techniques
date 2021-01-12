<template>
    <footer class="footer" id="footer">
        <div class="container is-fullhd">
            <div class="columns footer-links">
                <div class="column has-text-left">
                    <h2>Despre Kuppa</h2>
                    <ul>
                        <li>
                            <router-link :to="{ name: 'about' }"> Despre Noi </router-link>                            
                        </li>
                        <li>
                            <router-link :to="{ name: 'contact' }"> Contact </router-link>
                        </li>
                    </ul>
                </div>
                <div class="column has-text-left">
                    <h2>Integrari</h2>
                     <ul>
                         <li>
                             <a href=""> Woocommerce </a>
                        </li>
                        <li>
                            <a href=""> Shopify </a>
                        </li>
                        <li>
                            <a href=""> MerchantPro </a>
                        </li>
                        <li>
                            <a href=""> Magento 2 </a>
                        </li>
                        <li>
                            <a href=""> Wix </a>
                        </li>
                    </ul>             
                </div>
                <div class="column has-text-left">
                    <h2>Resurse</h2>
                   <ul>
                       <li>
                           <a href="https://kuppa.eu/info" target="_blank" rel="noopener"> Blog </a>
                        </li>
                        <li>
                            <a href=""> Help Center </a>
                        </li>
                        <li>
                            <a href=""> Intrebari Frecvente </a>
                        </li>
                    </ul>
                </div>
                <div class="column has-text-left">
                    <a href="/home" class="logo"><img src="@/assets/img/kuppa-footer.png?auto=compress,format&amp;rect=0,0,389,133&amp;w=102&amp;h=35" alt="logo kuppa"></a>
                    <p>Start a business and design the life you want – all in one place.</p>
                    <ul class="footer-social-media">
                        <li>
                            <a href="https://fb.me/kuppa.global" target="_blank" rel="noopener">
                                <img src="@/assets/img/facebook.svg" alt="facebook">
                            </a>
                        </li>
                        <li>
                            <a href="https://www.instagram.com/kuppashop/" target="_blank" rel="noopener">
                                <img src="@/assets/img/instagram.svg" alt="instagram">
                            </a>
                            </li>
                        <li>
                            <a href="https://www.linkedin.com/company/kuppa-shoop/about/" target="_blank" rel="noopener">
                                <img src="@/assets/img/linkedin.svg" alt="linkedin">
                            </a>
                        </li>
                    </ul>
                </div>
            </div>
        
            <div class="columns">
                <div class="column has-text-left copyright">
                    © 2020 Kuppa. Toate drepturile rezervate. Developed by <a href="http://lily.agency" target="blank">Lily Agency</a>
                </div>

                <div class="column has-text-right privacylinks">
                    <ul>
                        <li>
                            <router-link :to="{ name: 'privacy' }"> Politica de Confidentialitate </router-link>
                        </li>
                        <li>
                            <router-link :to="{ name: 'terms' }"> Termeni si Conditii </router-link>
                        </li>
                        <li>
                            <router-link :to="{ name: 'cookie' }"> Cookie Policy </router-link>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </footer>

</template>

<script>
export default {
  name: 'Footer',
};
</script>

<style lang="scss">
footer {
    &.footer {
        background-color:#03002f;
        color:#cccbcb;
        font-size:0.8rem;
        padding: 5rem 0 2rem;
        letter-spacing: 0.2px;
        font-weight: 200;
        clear: both;
        overflow: hidden;
    } 
    ul {        
        &.footer-social-media {
            margin-top:1.5rem;
            li {
                display:inline-block;
                padding:0 20px 0 0;
                a {
                    img {
                        height:30px;
                    }
                }
            }
        }
    }
    .footer-links {
        font-weight: 600;
        margin-bottom:3rem !important;
        h2 {
            margin-bottom: 1rem;
            color: #e8e8e8;
            font-size: 1rem;
            font-weight: 700;
        }
        ul {
            li {
                margin-bottom:1rem;
                a {
                    color:#cccbcb;
                    &:hover {
                        color: #00a98e;
                    }
                }
            }
        }
        .logo {
            img {
                margin-bottom:0.5rem;
            }
        }
    }
    .copyright {        
        a {
            color:#00a98e;
            &:hover {
                color:#cccbcb;
            }
        }
    }  
    .privacylinks {
        ul {
            li {
                display:inline-block;
                padding: 0 10px;
                a {
                    color:#cccbcb;
                    &:hover {
                        color: #00a98e;
                    }
                }
            }
        }
    } 
}
</style>

