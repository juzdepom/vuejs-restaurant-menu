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
    props: ['dishTypes'],
    components: {
        MenuSectionComponent: MenuSection,
    },
}
</script>

