<template>
    <div class="rm-back">
        <div class="rm-content">
            <menu-section-component :dishTypes="dishTypes"></menu-section-component>
        </div>
        <div class="rm-overlay"></div>
    </div>
</template>

<script>
import MenuSection from './MenuSection.vue'
export default {
    components: {
        MenuSectionComponent: MenuSection,
    },
    data(){
        return {
            dishTypes: [
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
            ]
        }
    }
}
</script>

