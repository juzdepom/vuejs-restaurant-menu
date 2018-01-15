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
    props: ['dishTypes'],
    components: {
        MenuSectionComponent: MenuSection,
    },
}
</script>

