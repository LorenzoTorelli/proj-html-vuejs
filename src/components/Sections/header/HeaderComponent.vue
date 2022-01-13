<template>
    <li class="header-bar">
        <div v-if="name == 'search'" class="searchBox">
            <a href="#">{{name}}</a>
            <input type="search" placeholder="Write here....">
        </div>
        
        <div class="item" v-else>
            <img :src="require( `../../../assets/svg/${logo}`)" alt="" v-if="logo">
            <a :href='link'>{{name}}</a>
        </div>
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
        .item {
            display: flex;
            a {
                text-decoration: none;
                text-transform: uppercase;
                color: white;
            }
            a:hover {
                text-decoration: underline;
            }
        }
        .searchBox {
            display: flex;
            align-items: center;
                a {
                    text-decoration: none;
                    text-transform: uppercase;
                    color: white;
            }
        }
        .searchBox input{
            background-color: black;
            border: none;
            outline: none;
            width: 0;
            padding: 0; 
            opacity: 0;
            border-bottom: 1px solid white;
            color: #fff;
            transition: all 1s;
        }




        .searchBox:hover input{
            width: 150px;
            opacity: 1;
            // display: block;
            padding: 0px 10px;
        }
        .searchBox:hover a {
            opacity: 0;
        }
        input {

            opacity: 0;
        }
        img {
            filter: invert(100%);
            margin-right: 5px;
            height: 20px;
            width: 20px;
        }
    }
</style>