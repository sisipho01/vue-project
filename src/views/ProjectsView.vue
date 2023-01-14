<template>
 <div class="work">
        <div v-for="project in Projects" :key="Projects" class="work">
            <div class="card" style="width: 18rem;">
            <img :src="project.img" class="d-block w-100" alt="..." >
                <div class="card-body">
                    <p class="card-title">{{ project.name }}</p>
                    <br>
                    <a :href="project.Netlify" class="btn btn-secondary">Netlify</a>
                </div>
            </div>
        </div>
</div>
</template>

<script>
export default {
    Projects: '',
    data(){
        return{
            Projects :[
                {
                name: 'Netflix',
                img:'https://i.postimg.cc/Gp6KTr3F/netflix.png',
                Netlify:'https://celebrated-jelly-72fca7.netlify.app/',
                },
                {
                name: 'Sisilator',
                img:'https://i.postimg.cc/9CHN2B6T/sisilator.png',
                Netlify:'https://sisilator.netlify.app/',
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
   .card{
    margin: 2rem 2rem;
    }
    .work{
        display: grid;
        grid-template-columns: 1fr 1fr 1fr;
    }

    @media screen and (max-width: 900px) {
        .work{
        display: grid;
        grid-template-columns: 1fr 1fr;
    }
    }
    @media screen and (max-width: 625px) {
        .work{
        display: grid;
        grid-template-columns: 1fr;
    }
    }
</style>