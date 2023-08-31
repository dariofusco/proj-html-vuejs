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
    </footer>
</template>

<style lang="scss" scoped>
footer {
    background-color: #18171f;
}

h5 {
    color: white;
}

ul, span {
    color: #696969;
}


</style>