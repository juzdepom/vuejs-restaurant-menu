<template>
  <div class="container">
			<section class="main">
				<div id="rm-container" class="rm-container">
					<div class="rm-wrapper">

						<menu-front-component :frontMenu="frontMenu" :leftMenu="leftMenu"></menu-front-component>
						<menu-middle-component :dishTypes="middleMenu"></menu-middle-component>
						<menu-right-component :dishTypes="rightMenu"></menu-right-component>

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
	},
	data(){
		return {
			frontMenu: {
				title: "Gourmet Castle",
				subtitle: "Fine Dining & Gourmet Takeaway",
				contact: {
					line1: "Gourmet Castle Restaurant",
					line2: "246 Wonderful Paradise Ln.",
					line3: "Pasadena, CA 91101",
					phone: "626.511.1170",
					fax: "626.992.1020",
				}
			}

			,
			leftMenu: [
                { title: "Appetizers",
                    dishes: [
                        {
                            name: "Bella's Artichokes",
                            des: "Roasted artichokes with chipotle aioli and cream cheese",
                        },
                        {
                            name: "Bruschetta Blue Delight",
                            des: "Blue cheese and citrus bruschetta",
                        },
                        {
                            name: "Pomme Dulse",
                            des: "Baked potatoes with crisped dulse",
                        },
                        {
                            name: "Green Love Crostini",
                            des: "Crostini with young pecorino, grilled figs and arugula &amp; mint pesto",
                        },
                        {
                            name: "Focaccia di Carciofi",
                            des: "Artichoke focaccia with fresh thyme",
                        },
                    ]

                },
                { title: "Salads & More",
                    dishes: [
                            {
                                name: "Green Delight",
                                des: "Watercress, frisee and avocado salad",
                            },
                            {
                                name: "Gourmet Yam Taohu",
                                des: "Thai tofu salad yam taohu",
                            },
                            {
                                name: "Panini Deluxe",
                                des: "Buffalo mozzarella basil panini",
                            },
                        ]

                }
			],
			middleMenu: [
                { title: "Main Courses",
                    dishes: [
                        {
                            name: "Crisspy Gnochi with Areoli",
                            des: "Roasted artichokes with chipotle aioli and cream cheese",
                        },
                        {
                            name: "Spicy Peanut Curry ",
                            des: "Tender sea palm noodles, seasoned vegetables, spicy peanut curry and tempeh fenel croquettes",
                        },
                        {
                            name: "Arugala",
                            des: "Dutch ginat oven-baked pancakes with sauteed apples",
                        },
                        {
                            name: "Glazed Tofu",
                            des: "Grilled marinated tofu, maple barbeque sauce, tahini slaw, grilled seasonal vegetables and mashed potatoes",
                        },
                        {
                            name: "Barbeque Tofu",
                            des: "Artichoke focaccia with fresh thyme",
                        },
                        {
                            name: "Luxury Oyster",
                            des: "King oyster mushroom with roasted cherries and sage",
                        },
                        {
                            name: "Rigatoni",
                            des: "Rigatoni with roasted cauliflower and spicy tomato sauce",
                        },
                        {
                            name: "Saffron Chana",
                            des: "Artichoke focaccia with fresh thyme",
                        },
                        {
                            name: "Steak with Onions",
                            des: "Saffron chickpea stew with grilled porcini mushrooms",
                        },
                    ]
                }
			],
			rightMenu: [
                { title: "Desserts",
                    dishes: [
                        {
                            name: "Crepes",
                            des: "Roasted artichokes with chipotle aioli and cream cheese",
                        },
                        {
                            name: "Pudding",
                            des: "Butterscotch pudding with bittersweet ganache and caramelize white chocolate crispies",
                        },
                        {
                            name: "Dutch Baby Sau",
                            des: "Dutch ginat oven-baked pancakes with sauteed apples",
                        },
                        {
                            name: "Blueberry Napoleon",
                            des: "Crostini with young pecorino, grilled figs and arugula &amp; mint pesto",
                        },
                        {
                            name: "Rings of Saturn",
                            des: "Artichoke focaccia with fresh thyme",
                        },
                        {
                            name: "Classic Atayet",
                            des: "Artichoke focaccia with fresh thyme",
                        },
                    ]
                }
            ]
		}
	}
}
</script>

