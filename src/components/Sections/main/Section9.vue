<template>
    <div id="sezione-9">
        <div class="container-fluid">
            <div class="row justify-content-center">
                <div class="col-lg-2 col-md-4 col-sm-12 ">
                    <input type="number" id="numeber" name="numer" min="1" placeholder="Number of person">
                    <h3>for</h3>
                </div>
                <div class="col-lg-2 col-md-4 col-sm-12">
                    <input type="date" id="date" name="date" placeholder="Date">
                    <h3>At</h3>
                </div> 
                <div class="col-lg-2 col-md-4 col-sm-12">
                    <input type="time" id="time" name="time" placeholder="Time">
                    <div class="btn"> BOOK A TABLE</div>
                </div>
            </div>
        </div>
        <!-- <p>* Powered by OpenTable</p> -->
    </div>
</template>

<script>
export default {
    name: "Section9"
}
</script>

<style lang="scss" scoped>
    #sezione-9 {
        color: white;
        background-image: url("../../../assets/Img/h3-background-img-3.jpg");
        padding: 80px 0px;
        margin-top: 10px;

        .row>div  {   
            display: flex;
            justify-content: center;
            align-items: center;

            input {
                padding: 10px ;
                margin: 0px 15px;
                border: 2px solid black;
            }
            h3 { 
                // align-self: center;
                text-transform: uppercase;
                font-size: 15px;
                margin-left: 50px;
            }
            .btn {
                padding: 10px;
                background-color: #d2401e;
                font-size: 15px;
                margin-left: 20px;
                color: white;
            }
        }
        p {
            font-size: 10px;
            margin-left: 35%;
        }

    }
</style>