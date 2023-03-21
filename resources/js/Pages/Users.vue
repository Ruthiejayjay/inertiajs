<template>
    <h1 class="text-3xl font-bold">Users</h1>

    <div style="margin-top: 600px">
      <p>The Current time is {{ time }}.</p>
      <Link href="/users" class="text-blue-500" preserve-scroll>Refresh</Link>
    </div>
</template>

<script>
    import { Link } from "@inertiajs/inertia-vue3";
    export default {
    components: { Link },
    props: { time: String },

    };
</script>
