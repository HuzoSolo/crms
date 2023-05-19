<template>
    <div class="section">
        
        <div class="row">
            <div class="col-8 p-0 m-0">
                <adminSectionsTable />
            </div>
            <div class="col-4 p-0 m-0">
                <adminSectionsRegisterPanel />
            </div>
        </div>
    </div>
</template>

<script>
    import adminSectionsRegisterPanel from './adminSectionsRegisterPanel.vue';
    import adminSectionsTable from './adminSectionsTable.vue';

    export default {
        components: {
            adminSectionsRegisterPanel,
            adminSectionsTable,
        },
    }
</script>

<style>

    .section{
        padding-top: 100px;
        padding-bottom: 100px;
    }


</style>