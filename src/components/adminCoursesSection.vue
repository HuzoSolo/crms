<template>
    <div class="section">
        
        <div class="row">
            <div class="col-8 p-0 m-0">
                <adminCoursesTable />
            </div>
            <div class="col-4 p-0 m-0">
                <adminCourseRegisterPanel />
            </div>
        </div>
    </div>
</template>

<script>
    import adminCoursesTable from './adminCoursesTable.vue';
    import adminCourseRegisterPanel from './adminCourseRegisterPanel.vue';

    export default {
        components: {
            adminCoursesTable,
            adminCourseRegisterPanel,
        },
    }
</script>

<style>

    .section{
        padding-top: 100px;
        padding-bottom: 100px;
    }


</style>