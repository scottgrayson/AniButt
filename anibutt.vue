<template>
    <div :class="addClass" class="btn">
        <span>{{content}}</span>
        <span v-show="loading"><i class="fa fa-spin fa-spinner"></i></span>
    </div>
</template>

<script>
    export default {
        props: {
            addClass: {
                default: 'btn-secondary'
            },
            loading: {
                type: Boolean,
                default: false
            },
            content: {
                default: 'content'
            }
        }
    }
</script>

