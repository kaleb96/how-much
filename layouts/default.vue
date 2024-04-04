<script setup lang="ts">

//state
const items = ref([
    {
        href: '/integration',
        title: '통합',
    },
    {
        href: '/maintenance',
        title: '관리비',
    },
    {
        href: '/gas',
        title: '가스비',
    },
    {
        href: '/subscribe',
        title: '구독료',
    },
    {
        href: '/info',
        title: '내 정보',
    },
    {
        href: '/signUp',
        title: '로그인',
    },
]);



</script>

<template>
    <a-typography-title>How much?</a-typography-title>
    <div class="container">
        <div class="content">
            <div class="header">
                <a-anchor class="anchor" direction="horizontal" :items="items" />
                <a-button>✏️</a-button>
            </div>
            <slot />
            <a-skleton active />
        </div>
    </div>

</template>

<style scoped>

.container {
    display: flex;
    justify-content: center;

}

.content {
    display: flex;
    flex-direction: column;
}
.header {
    display: flex;
    justify-content: space-between;
}

.anchor {
    width: 80vh;
    max-width: 80vh;
    min-width: 80vh;
}
</style>