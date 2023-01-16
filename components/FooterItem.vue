<template>
    <v-card flat class="mr-4">
        <v-icon>{{ icon }}</v-icon>
        <span>{{ name }}:&nbsp;</span>
        <a :href="link" target="_blank">{{ value }}</a>
    </v-card>
</template>

<script>
export default {
    props: {
        icon: String,
        name: String,
        link: String,
        value: String
    }
}
</script>
