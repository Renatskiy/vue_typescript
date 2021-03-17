<template>
  <div>
    <!-- <span @click="count">+</span> -->
    <span>{{ text }}</span>
  </div>
</template>

<script lang="ts">
import { Vue, Prop } from "vue-property-decorator";

export default class Counter extends Vue {
  @Prop({ default: "фывафывафыв" }) text!: string;

  //   public count = (): void => {
  //     this.concat();
  //   };
  //   public first = 1;
  //   public concat() {
  //     console.log(this.first);
  //     this.first++;
  //   }
}
</script>

<style lang="scss" scoped></style>
