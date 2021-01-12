<template>
    <header id="header" class="header">   
        <div class="container is-fluid">
            <div class="columns is-align-items-center">
                <div class="column has-text-left">                  
                    <a href="/" class="logo">
                        <img class="logo" src="../assets/img/logo-kuppa.png" alt="Kuppa Dropshipping">
                    </a>
                </div>
                <div class="column navigation">
                    <ul>
                        <li>
                            <router-link :to="{ name: 'dropshipping' }"> Dropshipping </router-link>
                        </li>
                        <li>
                            <router-link :to="{ name: 'integrations' }"> Integrations </router-link>
                        </li>
                        <li>
                            <router-link :to="{ name: 'products' }"> Products </router-link>
                        </li>
                        <li>
                            <router-link :to="{ name: 'pricing' }"> Pricing </router-link>
                        </li>
                    </ul>
                </div>

                <div class="column has-text-right loginregister">                    
                    <ul>
                        <li>
                            <a href="https://app.kuppa.global"> Login </a>
                        </li>
                        <li class="becomemember">
                            <a href="https://app.kuppa.global"> Become a Member </a>
                        </li>
                        <li>
                            <lang-dropdown />
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </header>

</template>

<script>
import LangDropdown from './LangDropdown.vue'

export default {
  name: 'Header',
  components: {
    LangDropdown
  },
};
</script>

<style lang="scss">
    header {
        .logo {
            img {
                height:30px;
            }
        }
        .navigation, .loginregister {
            ul {
                li {
                    display: inline;
                    padding:0 10px;
                    a {
                        color: #1d1d1f;
                        transition: 0.5s;
                        font-weight:600;
                         &:hover {
                        color: #00a98e;
                    }
                    }
                }
            }
        }
        .loginregister {
            ul {
                display: flex;
                align-items: flex-end;
                justify-content: flex-end;
                li {
                    &.becomemember{                      
                        a {
                            color:white;   
                            letter-spacing: 0.2px;
                            font-size: 0.8rem;
                            text-transform: uppercase;
                            font-weight: 700;      
                            background:#00a98e;
                            border-radius: 20px;
                            padding: 10px 20px 8px 20px;   
                            border:2px solid #00a98e;
                            transition: 0.7s;
                            &:hover {
                                background:transparent;
                                color: #00a98e;
                            }            
                        }
                    }
                    a {
                        font-size:0.9rem;
                    }
                }
            }
        }
    }
</style>

