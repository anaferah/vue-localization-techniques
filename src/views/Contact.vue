<template>
  <main id="contactpage" class="contactpage"> 
    <Header/>
        <div class="container is-fluid header-intro">
            <h2>Centrul&nbsp;de&nbsp;Asistenta&nbsp;clienti</h2>
            <p>Intra&nbsp;in&nbsp;contact&nbsp;cu&nbsp;echipa&nbsp;Kuppa.&nbsp;Suntem&nbsp;aici&nbsp;sa&nbsp;te&nbsp;ajutam.</p>
        </div>
        <div class="container contactoptions">
            <div class="columns">
                   <ul>
                       <li class="column">
                           <img src="@/assets/img/information.svg">
                           <h3>Help&nbsp;Center</h3>
                           <p>Rasfoieste articole&nbsp;utile,&nbsp;tutoriale informative,&nbsp;intrebari&nbsp;frecvente</p>
                           <a href=""><span>Detalii</span></a>
                        </li>
                        <li class="column">
                            <img src="@/assets/img/email.svg">
                            <h3>Vrei sa iei legatura cu noi?</h3>
                            <p>Scrie-ne un e-mail si iti vom raspunde in cel mai scurt timp posibil.</p>
                            <a href="mailto:info@kuppa.eu" target="_blank" rel="noopener"><span>Email</span></a>
                        </li>
                        <li class="column">
                            <img src="@/assets/img/add-user.svg">
                            <h3>Creaza cont</h3>
                            <p>Creaza un cont gratuit pe platforma Kuppa si bucura-te de beneficiile ce te asteapta.</p>
                            <a href="https://app.kuppa.global" target="_blank" rel="noopener"><span>Creaza cont</span></a>
                        </li>
                    </ul>
            </div>
        </div>
        <div class="container is-fluid insta">
            <div class="columns">
                <div class="column">
                    <div class="instatitle">
                        <a href="https://www.instagram.com/kuppashop/" target="_blank" rel="noopener">
                            <h3>Urmareste-ne pe Instagram @kuppa</h3>
                        </a>
                    </div>
                </div>
            </div>
             <div class="columns">
                <div class="column">
                    <a href="https://www.instagram.com/kuppashop/" target="_blank" rel="noopener">
                        <img src="https://images.prismic.io/kuppaweb/2f44df4e-15f9-49e3-912a-6858567cd1a0_bikeup.jpg?auto=compress,format">
                    </a>
                </div>
                <div class="column">
                    <a href="https://www.instagram.com/kuppashop/" target="_blank" rel="noopener">
                        <img src="https://images.prismic.io/kuppaweb/74963136-a13a-498a-aee6-822395febecc_wfh.jpg?auto=compress,format">
                    </a>
                </div>
                <div class="column">
                    <a href="https://www.instagram.com/kuppashop/" target="_blank" rel="noopener">
                        <img src="https://images.prismic.io/kuppaweb/053c2aee-ca9a-4682-b806-10f1f48026fb_work-office.jpg?auto=compress,format">
                    </a>
                </div>
                <div class="column">
                    <a href="https://www.instagram.com/kuppashop/" target="_blank" rel="noopener">
                        <img src="https://images.prismic.io/kuppaweb/89cc6ea9-97a4-44f3-b355-bdd3bbbb9834_work-cafe.jpg?auto=compress,format">
                    </a>
                </div>
                <div class="column">
                    <a href="https://www.instagram.com/kuppashop/" target="_blank" rel="noopener">
                        <img src="https://images.prismic.io/kuppaweb/c6ab316b-989b-4ee8-b8c5-cd89c61c0f96_selling.jpg?auto=compress,format">
                    </a>
                </div>
                <div class="column">
                    <a href="https://www.instagram.com/kuppashop/" target="_blank" rel="noopener">
                        <img src="https://images.prismic.io/kuppaweb/fd805591-7096-41da-8f8f-afa92e97d0fa_work-living.jpg?auto=compress,format">
                    </a>
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
  name: 'Contact',
  components: {
    Header,
    Footer
  }
}
</script>

<style lang="scss">
    #contactpage {
        .header-intro {
            h2 {
                font-size:3rem;
                font-weight:700;
                color:#1d1d1f;
            }
            p {
                color:#1d1d1f;
            }
        }
        .contactoptions {
            color:#1d1d1f;
            margin:5rem auto;
            h3 {
                color:#1d1d1f;
                font-size:1.3rem;
                font-weight:700;
            }
            p {
                color:#1d1d1f;
                margin:1rem 0 2rem;
            }
            img {
                height:50px;
            }
            span {
                border:2px solid #1d1d1d;
                padding:7px 25px 5px;
                color:#1d1d1f;
                font-weight: 600;
                transition: 0.5s;
            }
            ul {
                display:flex;
                li {
                    padding:2rem;
                }
            }
            a {
                &:hover {
                    span {
                        background:#1d1d1f;
                        color:white;
                    }                    
                }
            }
        }
        .insta {
            margin-bottom: 0rem;
            padding:0;
            .column {
                padding:0;
            }
            .instatitle {
                font-weight:800;
                font-size:1.2rem;
                color:#00a98e;
                margin-bottom:2rem;
                a {
                    color:#00a98e;
                    text-transform: uppercase;
                    h3 {
                        font-weight:700;
                    }
                }
            }
        }
    }
</style>

