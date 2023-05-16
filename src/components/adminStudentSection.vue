<template>

    <div class="section">
        <div class="row">
            <div class="col-8 p-0 m-0">
                <adminStudentTable />
            </div>
            <div class="col-4 p-0 m-0">
                <adminStudentRegisterPanel />
            </div>
        </div>
    </div>
</template>

<script>
import adminStudentTable from './adminStudentTable.vue';
import adminStudentRegisterPanel from './adminStudentRegisterPanel.vue';

export default {
    components: {
        adminStudentRegisterPanel,
        adminStudentTable,
    }
}
</script>

<style>

.section{
        padding-top: 100px;
        padding-bottom: 100px;
    }


</style>