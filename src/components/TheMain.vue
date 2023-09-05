<script>
import CardCourse from './CardCourse.vue';
import CardBlog from './CardBlog.vue';
export default {
    components: {
        CardCourse,
        CardBlog,
    },
    data() {
        return {
            courses: [
                {
                    img: "course-02-480x298.jpg",
                    price: "$40.00",
                    description: "Learning to Write as a Professional Author",
                    numberLessons: "20",
                    numberStudents: "50",
                },
                {
                    img: "stock-full-hd-03-480x298.jpg",
                    price: "$0.00",
                    description: "Customer-centric Info-Tech Strategies",
                    numberLessons: "24",
                    numberStudents: "769",
                },
                {
                    img: "stock-full-hd-04-480x298.jpg",
                    price: "$19.00",
                    description: "Open Programming Course for Everyone: Python",
                    numberLessons: "17",
                    numberStudents: "62",
                },
            ],
            blogs: [
                {
                    img: "artist-blog-03-480x325.jpeg",
                    name: "ARTIST",
                    description: "Brush Strokes Energize Trees in Paintings",
                    date: "May 15, 2020",
                    views: "688",
                },
                {
                    img: "artist-blog-01-480x325.jpg",
                    name: "ARTIST",
                    description: "Pocket-Sized Notebooks Hold Miniature Paintings",
                    date: "May 15, 2020",
                    views: "603",
                },
                {
                    img: "artist-blog-02-480x325.jpg",
                    name: "ARTIST",
                    description: "Connection Between Self-Portraits and Identity",
                    date: "May 15, 2020",
                    views: "397",
                },
            ],
        };
    },
    methods: {

    },
};
</script>

<template>
    <main>

        <!--Sezione Learn About-->
        <div class="bg-light">
            <div class="container py-5">
                <div class="row py-5">
                    <div class="col-3">
                        <span>EVERYTHING IN MAXCOACH</span>
                        <h3>Learn about our <span class="green">Work colture</span> at MaxCoach</h3>
                        <p>Spend some time to visit our website or head office and registration
                            deadline. We're opening new classes every beginning of each month.
                        </p>
                        <p>Have a questions? <a class="green" href="#">Get Free Guide <i
                                    class="fa-solid fa-arrow-right-long"></i></a></p>
                    </div>
                    <div class="col-3"></div>
                    <div class="col-6">
                        <img class="image"
                            src="../assets/img/stock-full-hd-10-ohki1ayywq3cqutettrncduujpoaorifqu4relt2ts.jpg" alt="">
                        <img class="overlap" src="../assets/img/about-us-01-ohkia3qg98rq9vg3s0mn2hkflr1migdqdw370qnegc.jpg"
                            alt="">
                    </div>
                </div>
                <div class="row py-5 text-center">
                    <div class="col"></div>
                    <div class="col-3">
                        <h2 class="green">129+</h2>
                        <span>ENROLLED LEARNERS</span>
                    </div>
                    <div class="col-3">
                        <h2 class="green">80</h2>
                        <span>FINISHED SESSIONS</span>
                    </div>
                    <div class="col-3">
                        <h2 class="green">4%</h2>
                        <span>SATISFACTION RATE</span>
                    </div>
                    <div class="col"></div>
                </div>
            </div>

            <!--Sezione Upgrade-->
            <div class="container py-5">
                <div class="row py-5">
                    <div class="col-6">
                        <img class="image" src="../assets/img/stock-full-hd-11-670x450.jpg" alt="">
                        <img class="yt-overlap" src="../assets/img/icon-youtube-play.png" alt="">
                    </div>
                    <div class="col-3"></div>
                    <div class="col-3">
                        <span>HOW WE WORK</span>
                        <h3>Upgrade Your Skills <span class="green">Upgrade Your Life</span></h3>
                        <p>Opening up more opportunities in front of you to get the ticket to
                            more enjoyable door in life. Getting equipped with new skills for new
                            sets of insights into your career. MaxCoach accompany learners in every stage
                            of learning.
                        </p>
                        <a href="#">Download free guidebook <i class="fa-solid fa-arrow-right-long"></i></a>
                    </div>
                </div>
            </div>

            <!--Sezione Latest Courses-->
            <div class="container py-5 text-center">
                <div class="row py-5">
                    <span>JOIN MAXCOACH AT BEST</span>
                    <h3>Latest Online <span class="green">Courses</span></h3>

                    <CardCourse v-for="singleCourse in courses" :img="singleCourse.img" :price="singleCourse.price"
                        :description="singleCourse.description" :numberLessons="singleCourse.numberLessons"
                        :numberStudents="singleCourse.numberStudents">
                    </CardCourse>

                    <p>Control your personal preference settings to get notified about appropriate courses.
                        <a href="#">View all courses <i class="fa-solid fa-arrow-right-long"></i></a>
                    </p>
                </div>
            </div>
        </div>

        <!--Sezione testimonials-->
        <div class="container py-5">
            <div class="row py-5">
                <div class="col-3">
                    <span>TESTIMONIALS</span>
                    <h3>Why Do People <span class="green">*Hearts*</span> Us?</h3>
                    <p>Seeking for verbals of our service quality? Find them here.
                        Everything is transparent and straightforward for your sense of justification.
                    </p>
                    <a href="#">View all <i class="fa-solid fa-arrow-right-long"></i></a>
                </div>
                <div class="col-2"></div>
                <div class="col-7">
                    <img class="image" src="../assets/img/immagine2023-09-01102152.jpg" alt="">
                </div>
            </div>
        </div>

        <!--Sezione everything-->
        <div class="container py-5">
            <div class="row py-5">
                <div class="col-6">
                    <img class="image" src="../assets/img/immagine2023-09-01102319.jpg" alt="">
                </div>
                <div class="col-3"></div>
                <div class="col-3">
                    <span>EVERYTHING IN MAXCOACH</span>
                    <h3>We're Here To <span class="green">Transform</span> You!</h3>
                    <p>As learners, people can enjoy great companionship from MaxCoach mentors
                        and educators. We can help you develop and grow at your best.
                    </p>
                    <button type="button" class="btn btn-success">Get Free Guide</button>
                </div>
            </div>
        </div>

        <!--Sezione latest Blog-->
        <div class="bg-light">
            <div class="container py-5">
                <div class="row py-5">
                    <span class="text-center">READ FOR MORE JOYMENT</span>
                    <h3 class="text-center">Latest From <span class="green">Our Blogs</span></h3>

                    <CardBlog v-for="singleBlog in blogs" :img="singleBlog.img" :name="singleBlog.name"
                        :description="singleBlog.description" :date="singleBlog.date" :views="singleBlog.views"></CardBlog>

                </div>
            </div>
        </div>
    </main>
</template>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;

.overlap {
    position: absolute;
    top: -80px;
    left: 480px;
    border-radius: 10%;
}

.yt-overlap {
    position: absolute;
    top: 180px;
    left: 300px;
}

.col-6 {
    position: relative;
}

.green {
    color: $primary_color;
}

a {
    color: black;
}

.card {
    width: 25rem;
    margin: 1rem;
    border: none;
}

.btn-success {
    background-color: $primary_color;
}
</style>