<template>
    <div class="container">
        <div class="items">
            <RecentActivity

            >
            <h3>{{ activity.title }}</h3>
            </RecentActivity>
        </div>

    </div>
</template>

<script>
import RecentActivity from './RecentActivity.vue';

    export default {
        name: 'ActivityComment',
        components: {
            RecentActivity
        },
            data() {
                return {
                    activities: [
                        {
                            title: 'Karen leave some comments on Konsep Ilustrasi',
                            date: '20 minutes ago'
                        },
                        {
                            title: 'Karen change project info on Project Homepage',
                            date: 'Yesterday'
                        },
                        {
                            title: 'Andrea change the due date of Project Homepage',
                            date: '23 June 2021'
                        },
                        {
                            title: 'Well done! You have submitted your tasks of Javascript 1',
                            date: '28 May 2021'
                        }
                    ]
                }
            },
    };
</script>