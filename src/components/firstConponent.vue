<template>
  <div>
    firstComponentfirstComponentfirstComponent
    <input type="text" v-model="textInput" />

    <Counter :text="text" />
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from "vue-property-decorator";
import Counter from "@/components/counter.vue";
@Component({
  components: {
    Counter,
  },
})
export default class FirstComponent extends Vue {
  public text = "texttext";

  get textInput() {
    return this.text;
  }
  set textInput(val: string) {
    this.text = val;
  }
}
</script>

<style lang="scss" scoped></style>
