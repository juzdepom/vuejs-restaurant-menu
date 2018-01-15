<template>
    <div class="rm-right">
        <div class="rm-back">
            <span class="rm-close" @click="close">Close</span>
            <div class="rm-content">
                <menu-section-component :dishTypes="dishTypes"></menu-section-component>
                <!-- <div class="rm-order">
                    <p><strong>Would you like us to cater your event?</strong> Call us &amp; we'll help you find a venue and organize the event: <strong>626.511.1170</strong></p>
                </div> -->
            </div>
        </div>
    </div>
</template>

<script>
import MenuSection from './MenuSection.vue'
export default {
    props: ['dishTypes'],
    methods: {
        close(){
            var container = $( '#rm-container' )
            container.removeClass( 'rm-open rm-nodelay rm-in' );
        }
    },
    components: {
        MenuSectionComponent: MenuSection,
    }
}
</script>

