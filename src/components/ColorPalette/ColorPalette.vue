<template>
  <mu-menu slot="right" placement="bottom-start" :open.sync="color" class="color"> 

    <mu-button icon class="right">
      <mu-icon value="palette" size="30"></mu-icon>
    </mu-button>

    <mu-list slot="content" class="list">
      <mu-list-item>
        <mu-list-item-action>
          <mu-avatar color="pink400" size="20" style="margin: 0 6px" button>
          </mu-avatar>
        </mu-list-item-action>
        <mu-list-item-content>
          <mu-list-item-title>Purple-Gold</mu-list-item-title>
        </mu-list-item-content>
      </mu-list-item>
    </mu-list>

  </mu-menu>
</template>

<script lang="ts">
import { Prop, Component, Vue } from 'vue-property-decorator';


@Component
export default class ColorPalette extends Vue {
  private color: boolean = false
}

</script>

<style lang="scss">
  .color {
    &:hover {
      color: $secondColor;
    }
  }
</style>