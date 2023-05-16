<template>
    <div class="mainFlow">
        <saluteUser></saluteUser>
        <coursesSection></coursesSection>
        <attendanceSection></attendanceSection>
        <control-panel></control-panel>
    </div>
</template>

<script>

import saluteUser from './saluteUser.vue';
import coursesSection from './coursesSection.vue';
import attendanceSection from './attendanceSection.vue';
import controlPanel from './controlPanel.vue';



export default {
    components: {
        saluteUser,
        coursesSection,
        attendanceSection,
        controlPanel,
    },

}
</script>

<style></style> 
