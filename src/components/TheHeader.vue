<script>
export default {
    data() {
        return {
            navLinks: [
                { name: "Home" },
                { name: "Pages" },
                { name: "Courses" },
                { name: "Features" },
                { name: "Blog" },
                { name: "Shop" },
            ],
        };
    },
};
</script>

<template>
    <header>

        <nav class="navbar">
            <div class="container-fluid">
                <ul class="navbar-nav">
                    <li class="nav-item" v-for="link in navLinks">
                        <a class="nav-link" href="#">{{ link.name }} <i class="fa-solid fa-chevron-down"></i></a>
                    </li>
                </ul>
                <a class="navbar-brand" href="#"><img class="logo" src="../assets/img/dark-logo.png" alt="logo"></a>
                <div class="input-group">
                    <i class="fa-solid fa-cart-shopping button"></i>
                    <i class="fa-solid fa-circle-user button"></i>
                    <input type="text" class="form-control" placeholder="Search..." aria-label="Search"
                        aria-describedby="button-addon2">
                    <button class="btn btn-outline-secondary" type="button" id="button-addon2"><i
                            class="fa-solid fa-magnifying-glass"></i></button>
                </div>
            </div>
        </nav>

    </header>
</template>

<style lang="scss" scoped>
.form-control {
    max-width: 10rem;
}

.logo {
    width: 200px;
}

.input-group{
    width: auto;
    align-items: center;
    padding-right: 2rem;
}

.navbar-nav {
    flex-direction: row;
}
.nav-item {
    padding-left: 2rem;
}

.button {
    padding-right: 2rem;
}
</style>