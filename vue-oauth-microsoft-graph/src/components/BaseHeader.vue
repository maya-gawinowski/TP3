<template>
    <div>    
        <div class="container">
            <div class="one">
                <div class="innerleft"><font-awesome-icon icon="fa-solid fa-house-user" transform="grow-30"/></div>
                <div class="innerright"> <h1>Home</h1></div>
            </div>
            <div class="two">
                <h1> Not yet logged-in</h1>
            </div>
            <div style="clear: both;"></div>
        </div>
    </div>
</template>

<style>
    .container {
        position: relative;
        align-items: center;
        background-color: #2bb883;
    }

    .one{
        float: left;
        align-items: center;
        padding: 20px;
    }

    .innerleft{
        float: left;
        padding: 20px;
    }

    .innerright{
        float: right;
        padding-left: 20px;
    }

    .two{
        float: right;
        padding: 20px;
    }

    .two, .innerright{
        font-family: "Gill Sans", sans-serif;
    }


</style>