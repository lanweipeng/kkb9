<template>
    <div>
        <label for="">{{label}}</label>
        <slot/>
    </div>
</template>
<script>
export default {
    props:['label']
}
</script>