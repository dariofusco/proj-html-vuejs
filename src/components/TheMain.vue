<script>
export default {

};
</script>

<template>
<main>

    <div class="hero text-center">
        <h3>Commence Business</h3>
        <h1>Distant Mentoring Program</h1>
        <button type="button" class="btn btn-light">Download free guidebook <i class="fa-solid fa-arrow-right-long"></i></button>
    </div>

    <div class="container py-5">
        <div class="row py-5">
            <div class="col-3">
                <span>EVERYTHING IN MAXCOACH</span>
                <h3>Learn about our <span>Work colture</span> at MaxCoach</h3>
                <p>Spend some time to visit our website or head office and registration
                    deadline. We're opening new classes every beginning of each month.
                </p>
                <p>Have a questions? <a href="#">Get Free Guide <i class="fa-solid fa-arrow-right-long"></i></a></p>
            </div>
            <div class="col-3"></div>
            <div class="col-6">
                <img class="image" src="../assets/img/stock-full-hd-10-ohki1ayywq3cqutettrncduujpoaorifqu4relt2ts.jpg" alt="">
                <img class="overlap" src="../assets/img/about-us-01-ohkia3qg98rq9vg3s0mn2hkflr1migdqdw370qnegc.jpg" alt="">
            </div>
        </div>
        <div class="row py-5 text-center">
            <div class="col"></div>
            <div class="col-3">
                <h2>129+</h2>
                <span>ENROLLED LEARNERS</span>
            </div>
            <div class="col-3">
                <h2>80</h2>
                <span>FINISHED SESSIONS</span>
            </div>
            <div class="col-3">
                <h2>4%</h2>
                <span>SATISFACTION RATE</span>
            </div>
            <div class="col"></div>
        </div>
    </div>

</main>
</template>

<style lang="scss" scoped>
.hero {
    background-image: url(../assets/img/home-3-hero-bg.jpg);
    height: 700px;
    padding: 250px;
    color: white;
}
.btn {
    color: #20ad96;
}

.overlap {
    position: absolute;
    top: -80px;
    left: 480px;
    border-radius: 10%;
}

.col-6 {
    position: relative;
}
</style>