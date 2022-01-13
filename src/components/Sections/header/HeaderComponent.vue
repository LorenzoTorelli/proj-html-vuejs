<template>
    <li class="header-bar">
        <img :src="require( `../../../assets/svg/${logo}`)" alt="" v-if="logo">
        <a :href='link'>{{name}}</a>
    </li>
</template>

<script>
export default {
    name:"HeaderComponent",
    props: {
        name: String,
        logo: String,
        link: String,
    },

}
</script>

<style lang="scss" scoped>
    li {
        display: flex;
        list-style: none;
        margin: 0px 10px;
        a {
            text-decoration: none;
            text-transform: uppercase;
            color: white;
        }
        a:hover {
            text-decoration: underline;
        }
        img {
            filter: invert(100%);
            margin-right: 5px;
            height: 20px;
            width: 20px;
        }
    }
</style>