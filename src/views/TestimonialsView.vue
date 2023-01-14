<template>
    <div class="container">
        <h2>Testimonials</h2>
        <p>Below is a character reference from people who have worked with me</p>
    </div>
    <div class="wrapper">

        <div v-for="Testimonial in Testimonials" :key="Testimonial" class="wrapper">
            <div class="card" style="width: 18rem;">
      <img :src=Testimonial.img class="card-img-top" alt="...">
      <div class="card-body">
        
        <p class="card-title">{{ Testimonial.name }}</p>
        <p class="card-title">{{ Testimonial.title }}</p>
        <p class="card-text">{{ Testimonial.test }}</p>
      </div>
    </div>
    </div>
    </div>
</template>

<script>
export default {
    Testimonials: "cards",
    data(){
        return{
            Testimonials:[
                {
                name: 'Oslin Johnson',
                title: 'Lecturer',
                img:'https://i.postimg.cc/76hx3ZVp/oslin.png',
                test:'Sisipho is someone who strives for success in her work. She always has a strong and positive attitude towards life, and is a great problem-solver. She is someone who very rarely needs assistance and gives her all to ensure that she is building a successful career for herself.'
                },
                {
                    name: 'Elizabeth Ramalatsoa',
                    title: 'Peer',
                    img:'https://i.postimg.cc/rwGFcbsY/Elizabeth.jpg',
                    test:'Sisipho is the hardest worker that I know. She always goes above and beyond of what is expected of her. One the best qualities that she possesses is determination. A truly amazing quality that not everyone possesses.',
                },
                {
                    name: 'Beyonce Leanord',
                    title: 'Peer',
                    img:'https://i.postimg.cc/3NDYqfz1/beyonce.png',
                    test:'Sisipho has been extremely responsive, pleasure to work with because of her attributes such as: being intelligent and going an extra mile in all programming challenges.',
                },
                {
                    name: 'Joel Mukanya',
                    title: 'Lecturer',
                    img:'https://i.postimg.cc/cLG4pZxn/joel.jpg',
                    test:'Sisipho is a hard working lady with a big heart. She is organized, efficient and extremely competent with excellent rapport with people of all ages. Her communication skills are excellent no matter if you are talking about verbal or written. Her most important quality is that she always keeps herself updated with new information .Its just amazing to work with such a kind personality.',
                },
                {
                    name: 'Zoe Daniels',
                    title: 'Peer',
                    img:'https://i.postimg.cc/G2fbqng9/zoe-daniels.jpg',
                    test:'Sisipho is an ambitious and a hard working woman. A very brilliant and bright woman, she always does her utmost best when it comes to her work. She always makes sure that she understands the work and if not she communicates to ask for guidance. Her personality is one of the things that builds her amazing character and I feel that she would be suitable and a good asset to any company that finds fit.',
                },
                {
                    name: 'Deno Rautenbach',
                    title: 'Peer',
                    img:'https://i.postimg.cc/bw18GYRP/deno.png ',
                    test:"Sisipho has an extremely attentive attention to detail when it comes to her work. Her designs aren't overly flamboyant and have shuttle care put into them that and especially helpful when working in Front end.",
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
    .wrapper{
        display: grid;
        grid-template-columns: 1fr 1fr 1fr;
    }

    @media screen and (max-width: 900px) {
        .wrapper{
        display: grid;
        grid-template-columns: 1fr 1fr;
    }
    }
    @media screen and (max-width: 625px) {
        .wrapper{
        display: grid;
        grid-template-columns: 1fr;
    }
    }
    
</style>