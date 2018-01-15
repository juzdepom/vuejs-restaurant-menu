<template>
    <div class="rm-right">
        <div class="rm-back">
            <span class="rm-close">Close</span>
            <div class="rm-content">
                <menu-section-component :dishTypes="dishTypes"></menu-section-component>
                <div class="rm-order">
                    <p><strong>Would you like us to cater your event?</strong> Call us &amp; we'll help you find a venue and organize the event: <strong>626.511.1170</strong></p>
                </div>
            </div>
        </div>
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

