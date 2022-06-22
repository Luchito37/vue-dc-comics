<template>
    <div class="my-4">
        <img :src="imgUrl" :alt="`${cardTitle}`" width="162" height="162">
        <div class="card-body text-white">{{cardTitle}}</div>
    </div>
</template>


<script>

export default{
    props: {
        cardTitle: String,
        imgUrl: String,
        isPrimary: Boolean,
    },
}
</script>
