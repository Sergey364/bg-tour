<template>
<a href="{{item.link}}" class="navigation-navbar__item" title="{{item.title}}">{{item.title}}</a>
</template>

<style scoped>
.navigation-navbar__item {
    display: flex;
    border-radius: 50%;
}

.navigation-navbar__item:hover {
    background-color: rgb(89, 124, 155)
}
</style>
