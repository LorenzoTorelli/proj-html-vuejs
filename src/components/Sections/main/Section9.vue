<template>
    <section id="section-9">
        <div class="container-fluid">
            <div class="row Myform-container">
                <div class="col-lg-2 col-md-4 col-sm-12 form-sing ">
                    <input type="number" id="number" name="numer" min="1" placeholder="Number of person">
                    <h3>for</h3>
                </div>
                <div class="col-lg-2 col-md-4 col-sm-12 form-sing">
                    <input type="date" id="date" name="date" placeholder="Date">
                    <h3>At</h3>
                </div> 
                <div class="col-lg-2 col-md-4 col-sm-12 form-sing">
                    <input type="time" id="time" name="time" placeholder="Time">
                    <a class="my-btn">book a table </a>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: "Section9"
}
</script>

<style lang="scss" scoped>
    #section-9 {
        color: white;
        background-image: url("../../../assets/Img/h3-background-img-3.jpg");
        padding: 80px 0px;
        margin-top: 10px;

        .Myform-container {
            justify-content: center;
            .form-sing  {   
                display: flex;
                input {
                    padding: 10px ;
                    margin: 0px 15px;
                    border: 2px solid black;
                }
                h3 { 
                    align-self: center;
                    text-transform: uppercase;
                    font-size: 15px;
                    margin-left: 50px;
                }
            }
            
        }
        p {
            font-size: 10px;
            margin-left: 35%;
        }

    }
</style>