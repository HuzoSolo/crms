<template>
  <div class="section">
    <div class="row">
      <div class="col-8 p-0 m-0">
        <adminTeachersTable />
      </div>
      <div class="col-4 p-0 m-0">
        <adminTeachersRegisterPanel />
      </div>
    </div>
  </div>
</template>

<script>
import adminTeachersTable from "./adminTeachersTable.vue";
import adminTeachersRegisterPanel from "./adminTeachersRegisterPanel.vue";

export default {
  components: {
    adminTeachersRegisterPanel,
    adminTeachersTable,
  },
};
</script>

<style>
.section {
  padding-top: 100px;
  padding-bottom: 100px;
}
</style>