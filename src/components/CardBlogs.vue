<script>
export default {
    props: {
        img: String,
        name: String,
        description: String,
        date: String,
        views: String,
    },
};
</script>

<template>
    <div class="card">
        <img class="card-img-top" :src="img" alt="course">
        <div class="card-body">
            <h6 class="px-1">{{ name }}</h6>
            <p class="px-1">{{ description }}</p>
            <span><i class="fa-regular fa-calendar px-1"></i>{{ date }}</span><span class="px-2"><i
                    class="fa-solid fa-eye px-1"></i>{{ views }} views</span>
        </div>
    </div>
</template>

<style lang="scss" scoped></style>