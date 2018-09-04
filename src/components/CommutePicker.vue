<template>
<div class="commute-picker">
    <form>
         <div class="form-group">
            <input type="text" class="form-control" id="workAddress" :placeholder="'Address ' + workIndex">
        </div>
        <TravelTypePicker></TravelTypePicker>
    </form>
</div>
</template>

<script>
import TravelTypePicker from "./TravelTypePicker.vue";

export default {
    name: 'CommutePicker', 
    props: ['workIndex'], 
    data: function (){
        return { 
            workAddress: "", 
        }; 
    }, 
    components: {
        TravelTypePicker
    }, 
}
</script>

<style scoped>
.commute-picker {
    color: rgb(159, 217, 107);
    background-color: rgb(9, 81, 105); 
    padding: 5px; 
    margin: 5px; 
    border: 5px solid rgb(9, 81, 105); 
    border-radius: 10px; 
}
</style>
