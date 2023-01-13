<template>
    <div class="container">
        <div class="row">
            <div class="col cardDisplay scrollspy mt-4">
                <div class="card" v-for="item in projectCards" :key="item">
                    <img :src="item.image" class="card-img-top" alt="...">
                    <div class="card-body">
                        <h5 class="card-title">{{ item.projectName }}</h5>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Projects',
    data() {
        return {
            projectCards: [
                {
                    image: 'https://i.postimg.cc/YqKcG3rV/Beans2021.png',
                    projectName: 'Slide The Beans Project',
                    githubLink: 'https://github.com/Jamie-Lee-Kinnear/Slide-The-Bean',
                    netlifyLink: 'https://kinnear20slide-the-beans.netlify.app'
                },
                {
                    image: 'https://i.postimg.cc/pXzHqScR/Calculator.png',
                    projectName: 'Calculator Project 2021',
                    githubLink: 'https://github.com/Jamie-Lee-Kinnear/Calculator-Exercise',
                    netlifyLink: 'https://kinnear20first-calculator.netlify.app'
                },
                {
                    image: 'https://i.postimg.cc/gcwd6jvw/Cards2022.png',
                    projectName: 'Professional Cards Project',
                    githubLink: 'https://github.com/CodeBeans2022/Cards',
                    netlifyLink: 'https://cards-2022.netlify.app'
                },
                {
                    image: 'https://i.postimg.cc/nrm6Ssk0/Carousel-Project.png',
                    projectName: 'Carousel Project',
                    githubLink: 'https://github.com/CodeBeans2022/Carousel_Project',
                    netlifyLink: 'https://leescarouselproject2022.netlify.app'
                },
                {
                    image: 'https://i.postimg.cc/gcfpypDg/Ecommerce-Project.png',
                    projectName: 'Ecommerce Project',
                    githubLink: 'https://github.com/CodeBeans2022/Ecommerce_Project2022',
                    netlifyLink: 'https://leesecommerceproject.netlify.app'
                },
                {
                    image: 'https://i.postimg.cc/Sj0gnDcG/Final-Project2021.png',
                    projectName: 'Portfolio Project 1',
                    githubLink: 'https://github.com/Jamie-Lee-Kinnear/Final-Project',
                    netlifyLink: 'https://jamie-lee-kinnear20.netlify.app'
                },
                {
                    image: 'https://i.postimg.cc/TYrzrDhP/My-Bakery.png',
                    projectName: 'My Bakery Project',
                    githubLink: 'https://github.com/CodeBeans2022/My-Bakery',
                    netlifyLink: 'my-bakery2022 https://my-bakery2022.netlify.app'
                },
                {
                    image: 'https://i.postimg.cc/mgB0VgFy/Portfolio-proj.png',
                    projectName: 'Portfolio Project 2',
                    githubLink: 'https://github.com/CodeBeans2022/Portfolio_2022',
                    netlifyLink: 'https://leesportfolio2022.netlify.app'
                },
                {
                    image: 'https://i.postimg.cc/gc6F25W8/Portfolio2022.png',
                    projectName: 'Portfolio Project 3',
                    githubLink: 'https://github.com/Jamie-Lee-Kinnear/Portfolio',
                    netlifyLink: 'https://kinnear20first-portfolio.netlify.app'
                },
                {
                    image: 'https://i.postimg.cc/t4k8cG3Q/Portfolioproj2.png',
                    projectName: 'Portfolio Project 4',
                    githubLink: 'https://github.com/Jamie-Lee-Kinnear/My-Porfolio',
                    netlifyLink: 'https://portfolio2-2021.netlify.app'
                },
                {
                    image: 'https://i.postimg.cc/Rh0GFdXW/POS2022.png',
                    projectName: 'POS Project 2022',
                    githubLink: 'https://github.com/CodeBeans2022/POS-Project',
                    netlifyLink: 'https://lees-pos2022.netlify.app/'
                },
                {
                    image: 'https://i.postimg.cc/tJmkV6M2/vue-E5.png',
                    projectName: 'Medicine Store',
                    githubLink: 'https://github.com/CodeBeans2022/Vue_Exercise5_Ec'
                },
                {
                    image: 'https://i.postimg.cc/KvWxDvkW/Grid-Calculator.png',
                    projectName: 'Grid Calculator',
                    githubLink: 'https://github.com/CodeBeans2022/Grid-Calculator',
                    netlifyLink: 'https://lees-calculator2022.netlify.app/'
                }
            ]
        }
    }
}


</script>

<style scoped>
img {
    height: 400px;
    width: 18rem;
    object-fit: cover;
}

.card {
    width: 18rem;
    height: 300px;
    margin: 10px;
}
.cardDisplay{
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
}

.scrollspy{
    overflow-y: scroll;
    height: 700px;
}
</style>