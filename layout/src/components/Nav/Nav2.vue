<template>
    <v-card class="mx-auto" max-width="">
    </v-card>
    <v-layout>
        <v-app-bar color="primary" density="compact">
        <!--density= comfortable (기본값), compact, loose, prominent-->
            <template v-slot:prepend>
                <v-app-bar-nav-icon></v-app-bar-nav-icon>
            </template>

        <v-app-bar-title>JINI</v-app-bar-title>
            <template v-slot:append>
                <v-btn icon="mdi-dots-vertical"></v-btn>
            </template>
        </v-app-bar>

        <v-main>
            <v-container fluid>
                <v-row>
                    <v-col
                    v-for="n in 8"
                    key="n"
                    cols="3">
                        <v-sheet
                        color="surface-variant-alt" height="96">
                        </v-sheet>
                    </v-col>
                </v-row>
            </v-container>
        </v-main>
    </v-layout>
</template>

<script setup>
</script>