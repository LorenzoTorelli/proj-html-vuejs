<template>
    <div id="section-5">
        <div class="card-container container-fluid">
            <div class="row">
                <div class="card col-lg-3 col-md-6 col-sm-12" v-for='(el,index) in team' :key='index'>
                    <img :src="require(`../../../assets/Img/${el.img}`)" :alt="el.img">
                    <div class="rect-hover">
                        <h4>{{el.name}}</h4>
                        <h5>{{el.role}}</h5>
                        <i class="fab fa-twitter"></i>
                        <i class="fab fa-facebook"></i>
                        <i class="fab fa-instagram"></i>
                    </div>
                </div>
            </div>
        </div>









    </div>
</template>

<script>
export default {
    name:"Section5",
    data() {
        return{
            team: [
                {
                    name:"Persona 1",
                    role:"Lavoro 1",
                    img:"h1-team-1a-700x700.jpg"
                },
                 {
                    name:"Persona 2",
                    role:"Lavoro 2",
                    img:"h1-team-2a.jpg"
                },
                 {
                    name:"Persona 3",
                    role:"Lavoro 3",
                    img:"h1-team-3a.jpg"
                },
                 {
                    name:"Persona 4",
                    role:"Lavoro 4",
                    img:"h1-team-4a.jpg"
                },

            ]
        }
    }
}
</script>

<style lang="scss" scoped>
    #section-5 {
        .card {
            padding: 0;
            position: relative;

            .rect-hover {
                transition: .5s ease;
                opacity: 0;
                position: absolute;
                top: 50%;
                left: 50%;
                transform: translate(-50%, -50%);
                text-align: center;
                color: white;
                padding: 25% 0%;
                width: 70%;
                height: 70%;
                background-color: #D2401E;
                border: 5px solid white;

                h4 {
                    font-size: 15px;
                    text-transform: uppercase;
                    font-weight: bold;
                }
                h5 {
                    font-size: 10px;
                    text-transform: uppercase;
                }
                i {
                    margin: 10px 5px;
                    cursor: pointer;
                }
            }
             &:hover img {
                opacity: 0.3;
                transition: .5s ease;

            }
            &:hover .rect-hover{
                opacity: 1;
            }
        }
    }
</style>