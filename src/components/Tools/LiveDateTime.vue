<template>
  <div class="text-subtitle-1 ml-3">
        {{ date }}
    </div>
</template>

<script>
import { format } from 'date-fns'
export default {
    data() {
        return {
            date: ''
        }
    },
    methods: {
        getDate() {
            this.date = format(new Date(), 'd MMMM, H:mm:ss')
            setTimeout(this.getDate, 1000)
        }
    },
    mounted() {
        this.getDate()
    }
}
</script>

<style>

</style>