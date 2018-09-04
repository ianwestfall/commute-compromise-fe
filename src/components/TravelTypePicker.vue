<template>
<div>
    <!-- Equally spaced inputs for each of the configured travel type options -->
    <div class="form-check form-check-inline" v-for="(option, index) in options" :key="index">
        <input class="form-check-input" type="radio" name="travelType" :id="id + option.value" :value="option.value" v-model="travelType">
        <label class="form-check-label" :for="id + option.value">{{ option.text }}</label>
    </div>
</div>
</template>

<script>
export default {
    name: 'TravelTypePicker', 
    data: function (){
        return { 
            travelType: "", 
            options: [
                { text: 'Car', value: 'car' },
                { text: 'Public Transit', value: 'public' },
                { text: 'Bike', value: 'bike' }
            ]
        }; 
    }, 
    mounted () {
        this.id = this._uid
    }
}
</script>

<style scoped>
</style>
