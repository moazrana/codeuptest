<template>
    <div id="banner">
        <div id="text-div">
            <h1>Welcome to Volex</h1>
            <p id="pera">Discover our wide range of products</p>
        </div>
    </div>
</template>

<script>
export default {

}
</script>

<style>
    #banner{
        /* background-color: aliceblue; */
        
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        background: url(/images/grey-abstract-background-wallpaper-design-free-vector-614940227.jpg);
        background-size: cover; /* To make sure the image covers the entire div */
        background-position: center; /* Center the image */
        background-repeat: no-repeat; /* Prevent repeating the image */
        width: 100%;
        height: 200px;
        padding: 0px;
        margin: 0px;
        gap: 0;
        
    }
    #pera{
        /* Discover our wide range of products */
        font-family: 'Instrument Sans';
        font-style: normal;
        font-weight: 500;
        font-size: 16px;
        line-height: 20px;
        /* identical to box height */

        color: rgba(26, 26, 26, 0.5);


        /* Inside auto layout */
        flex: none;
        order: 1;
        flex-grow: 0;

    }

</style>