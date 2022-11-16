<template>
    <div class="card-wrap">
        <img :src="cardIcon" alt="" role="presentation" />
        <h3> {{ cardHeading}} </h3>
        <p> {{ cardNote}} </p>
    </div>
</template>

<script>
export default {
    name: 'HerosheCard',
    props: [ 'cardIcon', 'cardHeading', 'cardNote']
}
</script>

<style scoped>
    .card-wrap {
        padding: 1rem;
        border-radius: 3px;
        background-color: #f5f5f5;
        margin-bottom: 1rem;
    }

    .card-wrap h3 {
        margin: 1rem 0;
    }
</style>