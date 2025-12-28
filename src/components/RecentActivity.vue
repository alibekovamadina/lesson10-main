<template>
    <div
        class="activity"
    >
        <div class="activity__icon">
            <img
                :src="activityImage"
                alt=""
            >
        </div>
        <div class="activity__info">
            <slot></slot>
            <p>{{ text }}</p>
        </div>
    </div>
</template>

<script>
    import ActivityComment from '@/components/ActivityComment.vue';

    export default {
        name: 'ResentActivity',
        props: [
            "title", "date"
        ],
        data() {
            return {
            }
        },
        computed: {
            activityClass() {
                return 'activity--' + this.title;
            activityImage() {
                return 'icon-' + this.title + .svg;
            }
            }
        },
        components: {
            ActivityComment
        }
    }
</script>