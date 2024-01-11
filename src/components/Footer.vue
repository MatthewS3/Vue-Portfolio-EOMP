<template>
    <div class="container0">
        <div class="row6">
            <p class="lead">
                Matthew's Portfolio &copy;
                <span> {{ currYear }} </span>
            </p>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'FooterComp',
        data() {
            return {
                currYear: new Date().getFullYear()
            }
        }
    }
</script>

<style>

</style>