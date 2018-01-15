<template>
  <div class="container">
			<section class="main">
				<div id="rm-container" class="rm-container">
					<div class="rm-wrapper">

						<menu-front-component></menu-front-component>
						<menu-middle-component></menu-middle-component>
						<menu-right-component></menu-right-component>

					</div><!-- /rm-wrapper -->
				</div><!-- /rm-container -->

			</section>

        </div>

</template>

<script>
import MenuFront from './MenuFront.vue'
import MenuMiddle from './MenuMiddle.vue'
import MenuRight from './MenuRight.vue'

export default {
  components: {
      MenuFrontComponent: MenuFront,
	  MenuRightComponent: MenuRight,
	  MenuMiddleComponent: MenuMiddle,
  }
}
</script>

