<template>
  <div id="navbar">
    <div>
        <p id="store-name"><span id="voxel">Voxel</span>Store</p>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style>
    #navbar{
        /* Navigation */

        /* Auto layout */
        display: flex;
        flex-direction: row;
        justify-content: space-between;
        align-items: center;
        padding: 0px;

        width: 1600px;
        height: 64px;


        /* Inside auto layout */
        flex: none;
        order: 0;
        align-self: stretch;
        flex-grow: 0;

    }
    #store-name{
        font-size: large;
    }
    #voxel{
        font-weight: bold;
    }
</style>