<script>
export default {
    props: {
        img: String,
        price: String,
        description: String,
        numberLessons: String,
        numberStudents: String,
    },
};
</script>

<template>
    <div class="card">
        <img class="card-img-top" :src="img" alt="course">
        <div class="card-body">
            <h4 class="green">{{ price }}</h4>
            <p>{{ description }}</p>
            <span class="px-2"><i class="fa-regular fa-file-zipper px-1"></i>{{ numberLessons }} Lessons</span>
            <span class="px-2"><i class="fa-regular fa-user px-1"></i>{{ numberStudents }} Students</span>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.green {
    color: #20ad96;
}
</style>