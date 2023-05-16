<template>
    <div class="section">
        
        <div class="row">
            <div class="col-8 p-0 m-0">
                <adminPaymentsTable />
            </div>
            <div class="col-4 p-0 m-0">
                <adminPaymentsRegisterPanel />
            </div>
        </div>
    </div>
</template>

<script>
    import adminPaymentsRegisterPanel from './adminPaymentsRegisterPanel.vue';
    import adminPaymentsTable from './adminPaymentsTable.vue';

    export default {
        components: {
            adminPaymentsRegisterPanel,
            adminPaymentsTable,
        },
    }
</script>

<style>

    .section{
        padding-top: 100px;
        padding-bottom: 100px;
    }


</style>