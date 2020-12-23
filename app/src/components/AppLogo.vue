<template>
    <img v-bind="$attrs" v-on="$listeners" v-bind:src="logo" alt="Logo" />
</template>

<script>
import logo from "../assets/logo.svg";

export default {
    data() {
        return {
            logo
        };
    }
}
</script>
