<template>
    <div class="site-bookmark">
        <a :href='href'>{{ text }}</a>
        <img :src="faviconUrl" :alt="text" />
    </div>
</template>

<script>
export default {
    props: {
        href: {
            type: String,
            required: true
        },
        text: {
            type: String,
            required: true
        }
    },
}
</script>

<style>
.site-bookmark {
    width: 169px;
    height: 169px;
    border-radius: 15px;
    background: #1E1E1E;
}
</style>
