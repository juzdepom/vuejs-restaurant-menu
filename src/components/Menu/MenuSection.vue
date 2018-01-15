<template>
    <div>
        <div v-for="(d, index) in dishTypes" :key="index">
            <h4 >{{d.title}}</h4>
            <dl>
                <div v-for="(dish, index) in d.dishes" :key="index">
                    <dt>{{dish.name}}</dt>
                    <dd>{{dish.des}}</dd>
                </div>
            </dl>
        </div>
    </div>
</template>

<script>
export default {
    props: ['dishTypes']
}
</script>
