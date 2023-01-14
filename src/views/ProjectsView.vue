<template>
    <div class="container" >
        <!-- <div id="carouselExampleControls" class="carousel slide" data-interval="false">
        <div id="carouselExampleCaptions" class="carousel slide" data-bs-ride="carousel">
            <div class="carousel-indicators">
                <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="0" class="active" aria-current="true" aria-label="Slide 1"></button>
                <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="1" aria-label="Slide 2"></button>
                <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="2" aria-label="Slide 3"></button>
                <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="3" aria-label="Slide 4"></button>
                <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="4" aria-label="Slide 5"></button>
                <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="5" aria-label="Slide 6"></button>
            </div>
        </div>
    </div>
     -->
   
            <!-- <div class="carousel-inner">
                <div v-for="Project in projectInner" :key="Project" class="carousel-item active">
                    <div class="card" style="width:18rem;">
                        <img :src="Project.img" class="d-block w-100" alt="..."> 
                        <div class="carousel-body">
                            <p class="carousel-caption">{{Project.name}}</p>
                            <br>
                            <a :href="Project.Netlify" class="btn btn-secondary">Netlify </a>
                        </div>
                    </div>  
                </div>
                <div v-for="project in Projects" :key="project" class="carousel-item">
                <div class="carousel" style="width: 18rem;">
                    <img :src="project.img" class="d-block w-100" alt="..." loading="lazy">
                    <div class="carousel-body">
                        <p class="card-title">{{ project.name }}</p>
                        <br>
                        <a :href="project.Netlify" class="btn btn-secondary">Netlify</a>
                    </div>
                </div>
          </div>
          </div>
            

        <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide="prev">
            <span class="carousel-control-prev-icon" aria-hidden="true"></span>
            <span class="visually-hidden">Previous</span>
        </button>
        <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide="next">
            <span class="carousel-control-next-icon" aria-hidden="true"></span>
            <span class="visually-hidden">Next</span>
        </button>
    
    </div> -->

    <div class="container">
      <div id="carouselExampleControls" class="carousel slide" data-interval="false">
        <div class="carousel-inner">
          <div v-for="Project in projectInner" :key="Project" class="carousel-item active">
            <div class="card" style="width:18rem;">
                        <img :src="Project.img" class="d-block w-100" alt="..."> 
                        <div class="carousel-body">
                            <p class="carousel-caption">{{Project.name}}</p>
                            <br>
                            <a :href="Project.Netlify" class="btn btn-secondary">Netlify </a>
                        </div>
                    </div>  
          </div>
          <div v-for="project in Projects" :key="project" class="carousel-item">
            <div class="carousel" style="width: 18rem;">
                    <img :src="project.img" class="d-block w-100" alt="..." loading="lazy">
                    <div class="carousel-body">
                        <p class="card-title">{{ project.name }}</p>
                        <br>
                        <a :href="project.Netlify" class="btn btn-secondary">Netlify</a>
                    </div>
                </div>
          </div>
        </div>
        <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleControls" data-bs-slide="prev">
            <span class="carousel-control-prev-icon" aria-hidden="true"></span>
            <span class="visually-hidden">Previous</span>
        </button>
        <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleControls" data-bs-slide="next">
            <span class="carousel-control-next-icon" aria-hidden="true"></span>
            <span class="visually-hidden">Next</span>
        </button>
      </div>
</div>
</div>
</template>

<script>
export default {
    Projects: 'carousel',
    data(){
        return{
            projectInner:[
                {
                name: 'Sisilator',
                img:'https://i.postimg.cc/9CHN2B6T/sisilator.png',
                Netlify:'https://sisilator.netlify.app/',
                }
            ],

            Projects :[
                {
                name: 'Netflix',
                img:'https://i.postimg.cc/Gp6KTr3F/netflix.png',
                Netlify:'https://celebrated-jelly-72fca7.netlify.app/',
                },
                {
                name: 'Portfolio 1',
                img:'https://i.postimg.cc/8CfBS3dj/portfolio-1.png',
                Netlify:'https://stirring-fairy-b9dedb.netlify.app/',
                },
                {
                name: 'Sisilator',
                img:'https://i.postimg.cc/9CHN2B6T/sisilator.png',
                Netlify:'https://sisilator.netlify.app/',
                },
                {
                name: 'Latest portfolio',
                img:'https://i.postimg.cc/ht5bNgdk/portfolio.png',
                Netlify:'https://sisipho-portfolio.netlify.app',
                },
                {
                name: 'Netflix',
                img:'https://i.postimg.cc/Gp6KTr3F/netflix.png',
                Netlify:'https://celebrated-jelly-72fca7.netlify.app/',
                }
        
            ]
        }
    }

}
</script>

<style scoped>
   img{
        height: 20rem;
        object-fit: cover;
        object-position: top;
        width: 5rem;
    }
    .container{
        margin: auto;
        background-color:blue; 
    }
    .card{
        margin: auto;
        margin-top: 2rem;
        margin-bottom: 5rem;
        gap: 1rem;
        box-shadow: 0 0 25px #555;
    }
    .carousel-control-next-icon {
        background-image: url("data:image/svg+xml;charset=utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' fill='black' viewBox='0 0 8 8'%3E%3Cpath d='M2.75 0l-1.5 1.5 2.5 2.5-2.5 2.5 1.5 1.5 4-4-4-4z'/%3E%3C/svg%3E");
    }
    .carousel-control-prev-icon {
        background-image: url("data:image/svg+xml;charset=utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' fill='black' viewBox='0 0 8 8'%3E%3Cpath d='M5.25 0l-4 4 4 4 1.5-1.5-2.5-2.5 2.5-2.5-1.5-1.5z'/%3E%3C/svg%3E");
    }
</style>