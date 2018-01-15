<template>
    <div class="rm-middle">
        <div class="rm-inner">
            <div class="rm-content">
                <menu-section-component :dishTypes="dishTypes"></menu-section-component>
            </div>
            <div class="rm-overlay"></div>
        </div>
    </div>
</template>

<script>
import MenuSection from './MenuSection'
export default {
    components: {
        MenuSectionComponent: MenuSection,
    },
    data(){
        return {
            dishTypes: [
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
            ]
        }
    }
}
</script>

