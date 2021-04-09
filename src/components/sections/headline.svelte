<script lang="ts">
  export let src: string = "../assets/badges/PNG/acm-csuf-badge.png";
</script>

<div class="subpage-title-container">
  <object type="image/png" data="{src}" title="acm-csuf-logo"></object>
  <h1 class="brand-em"><slot /></h1>
</div>

<style lang="scss">
  @import "../../style/theme.scss";

  .subpage-title-container {
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: center;
  }

  .subpage-title-container object {
	width: 25px;
	height: 25px;
  }

  .subpage-title-container h1 {
	font-size: var(--min-h-font-size);
	padding-left: 18px;
  }

  @media screen and (max-width: 768px) {
    .subpage-title-container object {
      width: 250px;
	  height: 250px;
    }

	.subpage-title-container h1 {
	  font-size: var(--max-h-font-size);
	  padding-left: 48px;
	}
  }
</style>
