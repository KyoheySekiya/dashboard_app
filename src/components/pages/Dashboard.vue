<template>
  <div class="top">
    <value-card name="ユーザー数 合計" value="250" style="height: 250px; width: 350px;"></value-card>
    <value-card name="プレビュー数 合計" value="250" style="height: 250px; width: 450px;"></value-card>
    <value-card name="プレビュー数 合計" value="350" style="height: 350px; width: 870px;"></value-card>
    
  </div>
</template>
<script>
import ValueCard from "../molecules/ValueCard";
export default {
  components: {
    ValueCard
  }
};
</script>
<style scoped>
.top {
  padding: 0px 0 0 200px;
}
</style>