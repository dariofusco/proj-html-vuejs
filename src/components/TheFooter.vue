<script>
export default {
    data() {
        return {
            footerLinksAddress: [
                { name: "382 NE 191st St # 87394 Miami, FL 33179-3899" },
                { name: "+1(305) 547-9909 (9am - 5pm EST, Monday - Friday)" },
                { name: "support@maxcoach.com" },
            ],
            footerLinksExplore: [
                { name: "Start here" },
                { name: "Blog" },
                { name: "About us" },
                { name: "Success story" },
                { name: "Courses" },
                { name: "contact us" },
            ],
            footerLinksInformation: [
                { name: "Membership" },
                { name: "Purchase guide" },
                { name: "Privacy policy" },
                { name: "Terms of service" },
            ],
        };
    },
};
</script>

<template>
    <footer>

        <!--Sezione Subscribe-->
        <div class="container py-5 text-center">
            <div class="row py-5">
                <h1>Subscribe <span class="green">Newsletters</span></h1>
                <p>Enter your email address to register to our newsletter subscription delivered on a regular basis!</p>
                <div class="input-group mb-3 justify-content-center">
                    <input type="text" class="form-control" placeholder="Enter your email" aria-label="Enter your email"
                        aria-describedby="button-addon2">
                    <button class="btn btn-outline-secondary btn-success" type="button"
                        id="button-addon2">Subscribe</button>
                </div>
            </div>
        </div>

        <!--Footer's links-->
        <div class="bg-dark">
            <div class="container py-3">
                <div class="row">
                    <div class="col-4">
                        <h5>Address</h5>
                        <ul class="list-unstyled" v-for="link in footerLinksAddress">
                            <li>{{ link.name }}</li>
                        </ul>
                    </div>
                    <div class="col-4">
                        <h5>Explore</h5>
                        <ul class="list-unstyled" v-for="link in footerLinksExplore">
                            <li>{{ link.name }}</li>
                        </ul>
                    </div>
                    <div class="col-4">
                        <h5>Information</h5>
                        <ul class="list-unstyled" v-for="link in footerLinksInformation">
                            <li>{{ link.name }}</li>
                        </ul>
                    </div>
                </div>
                <div class="text-center">
                    <span><i class="fa-regular fa-copyright"></i> 2020 Maxcoach. All Rights Reserved</span>
                </div>
            </div>
        </div>
    </footer>
</template>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;
h5 {
    color: white;
}

ul,
span {
    color: #696969;
}

.green {
    color: $primary_color;
}

.form-control {
    max-width: 20rem;
}

.btn-success {
    background-color: $primary_color;
}
</style>