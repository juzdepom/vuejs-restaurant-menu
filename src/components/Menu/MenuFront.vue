<template>
    <div class="rm-cover">
        <div class="rm-front">
                <div class="rm-content">

                    <div class="rm-logo"></div>
                    <h2>{{frontMenu.title}}</h2>
                    <h3>{{frontMenu.subtitle}}</h3>

                    <a href="#" class="rm-button-open" @click="openMenu">View the Menu</a>
                    <div v-if="frontMenu.contact != null" class="rm-info">
                        <p>
                        <strong>{{frontMenu.contact.line1}}</strong><br>
                        {{frontMenu.contact.line2}}<br>
                        {{frontMenu.contact.line3}}<br>
                        <strong>Phone: </strong>{{frontMenu.contact.phone}}<br>
                        <strong>Fax: </strong>{{frontMenu.contact.fax}}</p>
                    </div>
                </div><!-- /rm-content -->
        </div><!-- /rm-front -->
        <menu-left-component :dishTypes="leftMenu" ></menu-left-component>
    </div>
</template>

<script>
import MenuLeft from './MenuLeft.vue'
export default {
    props: ['leftMenu', 'frontMenu'],
    components: {
        MenuLeftComponent: MenuLeft,
    },
    methods: {
        openMenu(){
            var container = $( '#rm-container' )
            container.addClass( 'rm-open' )
        }
    }
}
</script>

