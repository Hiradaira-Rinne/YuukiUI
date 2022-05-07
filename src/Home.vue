<template>
  <div>
    <div class="common-layout">
      <el-container>
        <el-aside width="200px">
          <public-aside/>
        </el-aside>
        <el-main>
          <router-view/>
        </el-main>
      </el-container>
    </div>
  </div>
</template>

<script>
import PublicAside from '@/components/aside/publicAside.vue'
export default {
  name: "home",
  components: {

    PublicAside: PublicAside
  },
}
</script>

<style scoped>

</style>