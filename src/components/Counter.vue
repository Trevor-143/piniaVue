<template >
    <div>
        <h3> {{count}} </h3>
    </div>
</template>

<script>
import { useCounterStore } from "@/stores/counter";

const counter = useCounterStore()
const count = counter.count

</script>