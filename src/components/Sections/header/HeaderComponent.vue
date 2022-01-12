<template>
    <li class="header-bar">
        <!-- <img :src="require( `../../../assets/svg/${logo}.svg`)" alt="" v-show="logo != ''"> -->
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
            height: 10%;
            width: 10%;
            // filter: invert(0);  
            // color: white;
        }
    }
</style>