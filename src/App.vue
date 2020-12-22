<template>
<div>
  <div v-if="estado">
  <!-- Navigation-->
  <nav class="navbar navbar-expand-lg sticky-top navbar-dark bg-primary ">            
        <a class="navbar-brand " href="# "> <img src="./assets/logo.jpg" width="30 " height="30
            " class="d-inline-block align-top " alt=" " loading="lazy ">
            Diagno Gestion
        </a>
        <div class="collapse navbar-collapse justify-content-end " id="navbarNav ">
            <ul class="navbar-nav ">
                <a class="nav-link" href="#informacion"> Informacion </a>
                <a class="nav-link" href="#casosexito"> Casos de exito </a>
                <a class="nav-link" href="#contacto"> Contacto </a>
                <a class="nav-link js-scroll-trigger" v-on:click="ingresar" href="# ">Sistema <span class="sr-only ">(current)</span></a>
            </ul>
        </div>
    </nav>
 <!-- Carousel-->
    <div id="carouselExampleCaptions" class="carousel slide" data-ride="carousel">
        <ol class="carousel-indicators">
            <li data-target="#carouselExampleCaptions" data-slide-to="0" class="active"></li>
            <li data-target="#carouselExampleCaptions" data-slide-to="1" class=""></li>
            <li data-target="#carouselExampleCaptions" data-slide-to="2" class=""></li>
        </ol>
        <div class="carousel-inner">
            <div class="carousel-item active">                 
                <a href="#informacion"><svg class="bd-placeholder-img bd-placeholder-img-lg d-block w-100" width="800" height="400" xmlns="http://www.w3.org/2000/svg" 
                  preserveAspectRatio="xMidYMid slice" focusable="false" role="img" aria-label="Placeholder: First slide"
                  src="../public/img/image3.jpg"></svg></a>
                <img src="../public/img/image3.jpg" >
                <div class="carousel-caption d-none d-md-block" style="position: absolute; left: 514px; width: 514px;">
                    <h5 class="subtitulo"><a href="#informacion">Informacion</a></h5>
                    <p class="contenido">Conocenos</p>
                </div>
            </div>
            <div class="carousel-item">
                <svg class="bd-placeholder-img bd-placeholder-img-lg d-block w-100" width="800" height="400" xmlns="http://www.w3.org/2000/svg" preserveAspectRatio="xMidYMid slice" focusable="false" role="img" aria-label="Placeholder: Second slide"><title>Placeholder</title>
                </svg>
                <img src="../public/img/image2.jpg">
                <div class="carousel-caption d-none d-md-block">
                    <h5 class="subtitulo"><a href="#casosexito">Casos de exito</a></h5>
                    <p class="contenido">Conoce algunos de nuestros clientes satisfechos</p>
                </div>
            </div>
            <div class="carousel-item">
                <a href="#contacto"><svg class="bd-placeholder-img bd-placeholder-img-lg d-block w-100" width="800" height="400" xmlns="http://www.w3.org/2000/svg"
                    preserveAspectRatio="xMidYMid slice" focusable="false" role="img" aria-label="Placeholder: Third slide">
                    </svg></a>
                   <img alt="contacto" src="../public/img/image1.jpg" >
                    <div class="carousel-caption d-none d-md-block">
                    <h5 class="subtitulo"><a href="#contacto">Contacto</a></h5>
                    <p class="contenido">Quieres comunicarte con nosotros dar click aqui</p>
                    </div>
            </div>
        <a class="carousel-control-prev" href="#carouselExampleCaptions" role="button" data-slide="prev">
            <span class="carousel-control-prev-icon" aria-hidden="true"></span>
            <span class="sr-only">Previous</span>
        </a>
        <a class="carousel-control-next" href="#carouselExampleCaptions" role="button" data-slide="next">
            <span class="carousel-control-next-icon" aria-hidden="true"></span>
            <span class="sr-only">Next</span>
        </a>
        </div>
     
         <!-- informacion-->
         <div class="container-fluid text-center bg-dark text-light" id="informacion">
              <h2 class="section-heading text-uppercase">informacion</h2>
          </div>
         <div class="container-fluid">
        <div class="row justify-content-center mb-5">
            <div class="col-sm-6 col-xs-12 col-lg-4 mt-5">
              
            
                <div class="card bg-light">
                        <div class="d-flex justify-content-center p-2">
                          <img :src="'https://i.imgur.com/r2oz9Uw.jpg'" alt="Imagen de Mabel Amber en Pixabay" height="200" width="200">
                        </div>
                    <div class="card-body">
                        <h5 class="card-title content-center" align="center"></h5>
                        <p class="card-text" align="center"> Con el apoyo de un equipo de profesionales experimentados, nuestro servicios estratégicos se adaptan a las necesidades de todos tipos y tamaños de clientes. Desde pequeñas empresas recién creadas hasta grandes corporaciones entregamos resultados duraderos y cuantificables. Por favor póngase en contacto con nosotros para saber cómo Mi Sitio puede ayudar a su éxito en el futuro.</p>
                        <a href="https://liortiz.github.io/Pagina/#page-top" target="_blank" rel="noopener noreferrer" class="btn btn-primary"
                        > Mas informacion </a>
                    </div>
                </div>
            
            </div>
        </div>
    </div>

    
      <div class="container-fluid p-3 my-3 " >
        <!-- Services-->
        <section class="page-section" id="casosexito">
            <div class="container" >
                <h2 class="text-center mt-0">Las etapas que integran el Diagnóstico Administrativo pueden resumirse en:</h2>
                <hr class="divider my-4">
                <div class="row">
                    <div class="col-lg-3 col-md-6 text-center">
                        <div class="mt-5">
                            <svg class="svg-inline--fa fa-database fa-w-14 fa-4x text-primary mb-4" aria-hidden="true" focusable="false" data-prefix="fas" data-icon="database" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512" data-fa-i2svg=""><path fill="currentColor" d="M448 73.143v45.714C448 159.143 347.667 192 224 192S0 159.143 0 118.857V73.143C0 32.857 100.333 0 224 0s224 32.857 224 73.143zM448 176v102.857C448 319.143 347.667 352 224 352S0 319.143 0 278.857V176c48.125 33.143 136.208 48.572 224 48.572S399.874 209.143 448 176zm0 160v102.857C448 479.143 347.667 512 224 512S0 479.143 0 438.857V336c48.125 33.143 136.208 48.572 224 48.572S399.874 369.143 448 336z"></path></svg><!-- <i class="fas fa-4x fa-database text-primary mb-4"></i> Font Awesome fontawesome.com -->
                            <h3 class="h4 mb-2">Recopilación de información</h3>
                        </div>
                    </div>
                    <div class="col-lg-3 col-md-6 text-center">
                        <div class="mt-5">
                            <svg class="svg-inline--fa fa-diagnoses fa-w-20 fa-4x text-primary mb-4" aria-hidden="true" focusable="false" data-prefix="fas" data-icon="diagnoses" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 640 512" data-fa-i2svg=""><path fill="currentColor" d="M496 256c8.8 0 16-7.2 16-16s-7.2-16-16-16-16 7.2-16 16 7.2 16 16 16zm-176-80c48.5 0 88-39.5 88-88S368.5 0 320 0s-88 39.5-88 88 39.5 88 88 88zM59.8 364c10.2 15.3 29.3 17.8 42.9 9.8 16.2-9.6 56.2-31.7 105.3-48.6V416h224v-90.7c49.1 16.8 89.1 39 105.3 48.6 13.6 8 32.7 5.3 42.9-9.8l17.8-26.7c8.8-13.2 7.6-34.6-10-45.1-11.9-7.1-29.7-17-51.1-27.4-28.1 46.1-99.4 17.8-87.7-35.1C409.3 217.2 365.1 208 320 208c-57 0-112.9 14.5-160 32.2-.2 40.2-47.6 63.3-79.2 36-11.2 6-21.3 11.6-28.7 16-17.6 10.5-18.8 31.8-10 45.1L59.8 364zM368 344c13.3 0 24 10.7 24 24s-10.7 24-24 24-24-10.7-24-24 10.7-24 24-24zm-96-96c13.3 0 24 10.7 24 24s-10.7 24-24 24-24-10.7-24-24 10.7-24 24-24zm-160 8c8.8 0 16-7.2 16-16s-7.2-16-16-16-16 7.2-16 16 7.2 16 16 16zm512 192H16c-8.8 0-16 7.2-16 16v32c0 8.8 7.2 16 16 16h608c8.8 0 16-7.2 16-16v-32c0-8.8-7.2-16-16-16z"></path></svg><!-- <i class="fas fa-4x fa-diagnoses text-primary mb-4"></i> Font Awesome fontawesome.com -->
                            <h3 class="h4 mb-2">Análisis organizacional o administrativo</h3>
                        </div>
                    </div>
                    <div class="col-lg-3 col-md-6 text-center">
                        <div class="mt-5">
                            <svg class="svg-inline--fa fa-list-ul fa-w-16 fa-4x text-primary mb-4" aria-hidden="true" focusable="false" data-prefix="fas" data-icon="list-ul" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512" data-fa-i2svg=""><path fill="currentColor" d="M48 48a48 48 0 1 0 48 48 48 48 0 0 0-48-48zm0 160a48 48 0 1 0 48 48 48 48 0 0 0-48-48zm0 160a48 48 0 1 0 48 48 48 48 0 0 0-48-48zm448 16H176a16 16 0 0 0-16 16v32a16 16 0 0 0 16 16h320a16 16 0 0 0 16-16v-32a16 16 0 0 0-16-16zm0-320H176a16 16 0 0 0-16 16v32a16 16 0 0 0 16 16h320a16 16 0 0 0 16-16V80a16 16 0 0 0-16-16zm0 160H176a16 16 0 0 0-16 16v32a16 16 0 0 0 16 16h320a16 16 0 0 0 16-16v-32a16 16 0 0 0-16-16z"></path></svg><!-- <i class="fas fa-4x fa-list-ul text-primary mb-4"></i> Font Awesome fontawesome.com -->
                            <h3 class="h4 mb-2">Obtención de conclusiones</h3>
                        </div>
                    </div>
                    <div class="col-lg-3 col-md-6 text-center">
                        <div class="mt-5">
                            <svg class="svg-inline--fa fa-lightbulb fa-w-11 fa-4x text-primary mb-4" aria-hidden="true" focusable="false" data-prefix="fas" data-icon="lightbulb" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 352 512" data-fa-i2svg=""><path fill="currentColor" d="M96.06 454.35c.01 6.29 1.87 12.45 5.36 17.69l17.09 25.69a31.99 31.99 0 0 0 26.64 14.28h61.71a31.99 31.99 0 0 0 26.64-14.28l17.09-25.69a31.989 31.989 0 0 0 5.36-17.69l.04-38.35H96.01l.05 38.35zM0 176c0 44.37 16.45 84.85 43.56 115.78 16.52 18.85 42.36 58.23 52.21 91.45.04.26.07.52.11.78h160.24c.04-.26.07-.51.11-.78 9.85-33.22 35.69-72.6 52.21-91.45C335.55 260.85 352 220.37 352 176 352 78.61 272.91-.3 175.45 0 73.44.31 0 82.97 0 176zm176-80c-44.11 0-80 35.89-80 80 0 8.84-7.16 16-16 16s-16-7.16-16-16c0-61.76 50.24-112 112-112 8.84 0 16 7.16 16 16s-7.16 16-16 16z"></path></svg><!-- <i class="fas fa-4x fa-lightbulb text-primary mb-4"></i> Font Awesome fontawesome.com -->
                            <h3 class="h4 mb-2">Propuesta y plan de acción</h3></div>
                        </div>
               </div>
          </div>
            
        </section>
      </div>
      <div class="container-fluid text-center bg-dark text-light">
              <h2 class="section-heading text-uppercase">Casos exitosos</h2>
          </div>
      <home-2/>
      </div>
      <!-- Contact-->
        <section class="page-section" id="contacto">
            <div class="container">
                <div class="row justify-content-center">
                    <div class="col-lg-5 text-center">
                        <h2 class="mt-0">Diagno Gestion!</h2>
                        <hr class="divider my-4">
                        <p class="text-muted mb-5">Te permite solucionar tus problemas en tu empresa</p>
                    </div>
                </div>
                <div class="row">
                    <div class="col-lg-4 ml-auto text-center mb-5 mb-lg-0">
                        <svg class="svg-inline--fa fa-phone fa-w-16 fa-3x mb-3 text-muted" aria-hidden="true" focusable="false" data-prefix="fas" data-icon="phone" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512" data-fa-i2svg=""><path fill="currentColor" d="M493.4 24.6l-104-24c-11.3-2.6-22.9 3.3-27.5 13.9l-48 112c-4.2 9.8-1.4 21.3 6.9 28l60.6 49.6c-36 76.7-98.9 140.5-177.2 177.2l-49.6-60.6c-6.8-8.3-18.2-11.1-28-6.9l-112 48C3.9 366.5-2 378.1.6 389.4l24 104C27.1 504.2 36.7 512 48 512c256.1 0 464-207.5 464-464 0-11.2-7.7-20.9-18.6-23.4z"></path></svg><!-- <i class="fas fa-phone fa-3x mb-3 text-muted"></i> Font Awesome fontawesome.com -->
                        <div>+57 (310) 123-4567</div>
                    </div>
                    <div class="col-lg-4 mr-auto text-center">
                        <svg class="svg-inline--fa fa-envelope fa-w-16 fa-3x mb-3 text-muted" aria-hidden="true" focusable="false" data-prefix="fas" data-icon="envelope" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512" data-fa-i2svg=""><path fill="currentColor" d="M502.3 190.8c3.9-3.1 9.7-.2 9.7 4.7V400c0 26.5-21.5 48-48 48H48c-26.5 0-48-21.5-48-48V195.6c0-5 5.7-7.8 9.7-4.7 22.4 17.4 52.1 39.5 154.1 113.6 21.1 15.4 56.7 47.8 92.2 47.6 35.7.3 72-32.8 92.3-47.6 102-74.1 131.6-96.3 154-113.7zM256 320c23.2.4 56.6-29.2 73.4-41.4 132.7-96.3 142.8-104.7 173.4-128.7 5.8-4.5 9.2-11.5 9.2-18.9v-19c0-26.5-21.5-48-48-48H48C21.5 64 0 85.5 0 112v19c0 7.4 3.4 14.3 9.2 18.9 30.6 23.9 40.7 32.4 173.4 128.7 16.8 12.2 50.2 41.8 73.4 41.4z"></path></svg><!-- <i class="fas fa-envelope fa-3x mb-3 text-muted"></i> Font Awesome fontawesome.com -->
                        <!-- Make sure to change the email address in BOTH the anchor text and the link target below!-->
                        <a class="d-block" href="mailto:contact@yourwebsite.com">contact@diagnogestion.com</a>
                    </div>
                </div>
            </div>
        </section>
     
    <!-- Footer-->
        <footer class="bg-light text-center text-lg-start">
            <div class="container"><div class="small text-center text-muted">Copyright © 2020</div></div>
        </footer>
    
 <div class="mc1inlineContent" id="comp-kizi4fm42inlineContent" style="width: 100%; position: absolute; top: 0px; bottom: 0px;">
        <div data-content-area-marker="comp-kizi4fm42" data-aid="content-area-marker-comp-kizi4fm42" style="visibility: hidden; 
        position: absolute; width: 300px; margin-left: calc((100% - 300px) * 0.5);">
        </div></div>
    
  </div>
  <div v-else>
  <v-app id="app">
    <v-navigation-drawer
      v-model="drawer"
      :clipped="$vuetify.breakpoint.lgAndUp"
      app
    >
      <v-list dense>
        <template>
          <v-list-item @click="home">
            <v-list-item-action>
              <v-icon>home</v-icon>
            </v-list-item-action>
            <v-list-item-title>
              Inicio
            </v-list-item-title>
          </v-list-item>
        </template>
        <template v-if="logueado">
          <v-list-group>
            <v-list-item slot="activator">
              <v-list-item-content>
                <v-list-item-title>
                  Almacén
                </v-list-item-title>
              </v-list-item-content>
            </v-list-item>
            <v-list-item :to="{name: 'categoria'}">
              <v-list-item-action>
                <v-icon>table_chart</v-icon>
              </v-list-item-action>
              <v-list-item-content>
                <v-list-item-title>
                  Categorías
                </v-list-item-title>
              </v-list-item-content>
            </v-list-item>
            <v-list-item :to="{name: 'articulo'}">
              <v-list-item-action>
                <v-icon>table_chart</v-icon>
              </v-list-item-action>
              <v-list-item-content>
                <v-list-item-title>
                  Artículos
                </v-list-item-title>
              </v-list-item-content>
            </v-list-item>
          </v-list-group>
          <v-list-group>
            <v-list-item slot="activator">
              <v-list-item-content>
                <v-list-item-title>
                  Accesos
                </v-list-item-title>
              </v-list-item-content>
            </v-list-item>
            <v-list-item :to="{name: 'usuario'}">
              <v-list-item-action>
                <v-icon>table_chart</v-icon>
              </v-list-item-action>
              <v-list-item-content>
                <v-list-item-title>
                  Usuarios
                </v-list-item-title>
              </v-list-item-content>
            </v-list-item>
          </v-list-group>
        </template> 
      </v-list>
    </v-navigation-drawer>

    <v-app-bar
      :clipped-left="$vuetify.breakpoint.lgAndUp"
      app
      color="silver darken-3"
      dark
    >
      <v-toolbar-title
        style="width: 300px"
        class="ml-0 pl-3"
      >
        <v-app-bar-nav-icon @click.stop="drawer = !drawer"></v-app-bar-nav-icon>
        <span class="hidden-sm-and-down">Sistema</span>
      </v-toolbar-title>      
      <v-spacer></v-spacer>
      <v-btn @click="salir()" icon v-if="logueado">
        <v-icon>logout</v-icon> Salir
      </v-btn>
      <v-btn :to="{name: 'login'}" icon v-else>
        <v-icon>apps</v-icon> Login
      </v-btn>
    </v-app-bar>
    <v-content>
      <v-container
        fluid
        fill-height
      >
        <v-slide-y-transition mode="out-in">
          <router-view/>
        </v-slide-y-transition>
      </v-container>
    </v-content>
    <v-footer height="auto">
      <v-layout justify-center>
        <v-flex text-xs-center>
          <v-card flat tile color="primary" class="white--text">
            <v-card-text class="white--text pt-0">
              Proyecto final &copy;2020
            </v-card-text>
          </v-card>
        </v-flex>
      </v-layout>
    </v-footer>
  </v-app>
  </div>
  </div>
</template>

<script>
import Home from './components/home.vue';
import home2 from './components/home2.vue'
export default {
  components: { home2, Home },
  name: 'App',

    data () {
      return {
      drawer: false,
      estado:1
      }
    },

  computed:{
    logueado(){
      return this.$store.state.usuario;
    },
  },
  created(){
    this.$store.dispatch("autoLogin");
  },
  methods:{
    salir(){
      this.$store.dispatch("salir");
      this.estado=1
    },

    ingresar(){
      this.estado=0
    },

    home(){
      this.estado=1

    }
  }
};
</script>