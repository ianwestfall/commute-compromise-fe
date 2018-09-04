<template>
<div class="container compromiser">
    <div class="row">
        <CommutePicker workIndex=1 class="col"></CommutePicker>
        <CommutePicker workIndex=2 class="col"></CommutePicker>
        
    </div>
    <div class="row">

        <!-- This is dummy crap until I actually integrate with Google Maps. --> 
        <div class="col map">
            <div class="mapouter">
                <div class="gmap_canvas">
                    <iframe width="600" height="500" id="gmap_canvas" src="https://maps.google.com/maps?q=washington%20dc&t=&z=13&ie=UTF8&iwloc=&output=embed" frameborder="0" scrolling="no" marginheight="0" marginwidth="0"></iframe>
                </div>
            </div>
        </div>
    </div>
    <div class="text-center">
        <button type="button" class="btn go-button">Go!</button>
    </div>
</div>
</template>

<script>
import CommutePicker from "./CommutePicker.vue";

export default {
    name: 'CommuteCompromise',
    components: {
        CommutePicker
    }, 
}
</script>

<style scoped>
    .compromiser {
        color: rgb(12, 6, 54);
        padding-bottom: 50px; 
    }

    .map {
        background-color: rgb(9, 81, 105);  
        border: 5px solid rgb(9, 81, 105); 
        border-radius: 10px; 
    }

    .go-button {
        color: rgb(159, 217, 107);
        background-color: rgb(9, 81, 105);
        border: 1px solid rgb(159, 217, 107);
        border-radius: 10px; 
        margin: 10px; 
        width: 50%; 
    }
</style>
