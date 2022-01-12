<template>
    <div id="sezione-9">
        <div class="container">
            <input type="number" id="numeber" name="numer" min="1" placeholder="Number of person">
            <h3>for</h3>
            <input type="date" id="date" name="date" placeholder="Date">
            <h3>At</h3>
            <input type="time" id="time" name="time" placeholder="Time">
            <div class="btn"> BOOK A TABLE</div>
        </div>
        <p>* Powered by OpenTable</p>
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

        .container  {

            display: flex;
            justify-content: center;
            align-items: center;

            input {
                padding: 10px ;
                margin: 0px 15px;
                border: 1px solid black;
            }
            h3 { 
                // align-self: center;
            }
            .btn {
                padding: 10px;
                background-color: #d2401e;
                font-size: 15px;
                margin-left: 20px;
            }
        }
        p {
            font-size: 10px;
            margin-left: 33%;
        }

    }
</style>