<template>
  <div id="section-1">
        <div class="card-container container-fluid">
            <div class="row">
                <div class="card col-lg-3 col-md-6 col-sm-12" v-for='(el,index) in img' :key='index'>
                    <img :src="require(`../../../assets/Img/${el.path}`)" :alt="el.path">
                    <div class="hover-cross">
                        <i class="fas fa-plus"></i>
                    </div>
                </div>
            </div>
        </div>

  </div>
</template>

<script>
export default {
    name:"Section-1",
    data() {
        return {
            img: [
                {
                path:"h3-img-1.jpg",
                },
                {
                path:"h3-img-2.jpg",
                },
                {
                path:"h3-img-3.jpg",    
                },
                {
                path:"h3-img-4.jpg",
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
    #section-1 {
        .card {
            padding: 0;
            position: relative;
            .hover-cross {
                transition: .5s ease;
                opacity: 0;
                position: absolute;
                top: 50%;
                left: 50%;
                transform: translate(-50%, -50%);
                -ms-transform: translate(-50%, -50%);
                text-align: center;
                color: white;
                padding: 15px 20px;
                background-color: #D2401E;
                border-radius: 50%;
                cursor: pointer;
            }
            &:hover img {
                opacity: 0.3;
                transition: .5s ease;

            }
            &:hover .hover-cross{
                opacity: 1;
            }
        }
            
    }
</style>