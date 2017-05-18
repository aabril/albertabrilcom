<template>
  <div v-on:click="onClick">
    <a role="button" class="" id="menuTrigger">
      <span class="line"></span>
      <span class="line"></span>
      <span class="line"></span>
    </a>
  </div>
</template>

<script>
export default {
  methods: {
    onClick: () => {

    }
  }
}
</script>

<style lang="less" scoped>

#menuTrigger {
	z-index: 9999;
	display: block;
	position: fixed;
	top: 0;
	right: 0;
	height: 30px;
	width: 50px;
	margin: 30px;

  &:hover {
    #menuTrigger.active;
  }

}
.line {
	display: block;
	width: 40px;
	margin: 0 5px;
	height: 6px;
	border-radius: 3px;
	background: #333;
	position: absolute;
	-webkit-transition: -webkit-transform 0.40s, top 0.40s, bottom 0.40s, left 0.40s;
	transition: transform 0.40s, top 0.40s, bottom 0.40s, left 0.40s;
	left: 0;
	&:nth-child(1) {
		top: 0;
	}
	&:nth-child(2) {
		top: 12px;
	}
	&:nth-child(3) {
		bottom: 0;
	}
}

#menuTrigger.active {
	.line {
		&:nth-child(1) {
			top: 12px;
			transform: rotate(-45deg);
			-webkit-transform: rotate(-45deg);
		}
		&:nth-child(2) {
			top: 12px;
			// left: 200%;
      transition: opacity .30s ease-in-out;
      -moz-transition: opacity .30s ease-in-out;
     opacity: 0;



		}
		&:nth-child(3) {
			bottom: 12px;
			transform: rotate(45deg);
			-webkit-transform: rotate(45deg);
		}
	}
}

</style>
