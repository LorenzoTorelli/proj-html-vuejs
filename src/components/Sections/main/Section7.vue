<template>
    <div id="sezione-7">
        <div class="pizza" v-for="(el, index) in pizzaType" :key="index">
            <img :src="require( `../../../assets/Img/${el.img}`)" alt="">
            <h4>{{el.name}}</h4>
            <h5><span v-show="el.oldPrice != ''">{{el.oldPrice}} -</span> {{el.price}}</h5>
            <div class="sold" v-show="el.sold"><h5>sold</h5></div>
        </div>
    </div>
</template>

<script>
export default {
    name:"Section7",
    data() {
      return {
        pizzaType: [
            {
                img:"h3-product-img-1a-100x100.png",
                name:"Bismark",
                price:"$30.00",
                oldPrice:"$25.00",
                sold:false,
            },
            {
                img:"h3-product-img-2a-150x150.png",
                name:"Fiori di Zucca",
                price:"$7.00 - $50.00",
                oldPrice:"",
                sold:false,
            },
            {
                img:"h3-product-img-3a-150x150.png",
                name:"Valdostana",
                price:"$55.00",
                oldPrice:"",
                sold:true,
            },
            {
                img:"h3-product-img-4a-150x150.png",
                name:"Pizza Tartufata",
                price:"$45.00",
                oldPrice:"",
                sold:false,
            },
            {
                img:"h3-product-img-5a-150x150.png",
                name:"Francescana",
                price:"$25.00",
                oldPrice:"",
                sold:false,
            },

            {
                img:"h3-product-img-6a-100x100.png",
                name:"Campagnola",
                price:"$50.00 - $95.00",
                oldPrice:"",
                sold:false,
            },
        ]
      }
    }
}
</script>

<style lang="scss" scoped>
    #sezione-7 {
        display: grid;
        grid-template-columns: repeat(auto-fill,250px);
        grid-gap: 30px;
        justify-content: center;
        
        .pizza{
            // background-color: red;
            text-align: center;
            position: relative;
            margin-bottom: 100px;
            img {
                width: 200px;
            }
            h4 {
                margin-top: 15px;
                color:#B7903C;
                text-transform: uppercase;
            }
            h5 {
                color:#D2401E;
                span{
                    color: #D3CFAF;
                    text-decoration: line-through;

                }

            }
            &:hover {
                background-color: lightgrey;
                transition: 0.3s ease;
                cursor: pointer;
                border-radius: 25px;
            }
            .sold {
                position: absolute;
                width: 40px;
                height: 40px;
                top: 5%;
                right: 15%;
                background-color: #D2401E;
                border-radius: 50%;
                h5 {
                    margin-top: 30%;
                    color: white;
                    text-transform: uppercase;
                    font-size: 10px;
                }
            }
        }
    }
</style>