<template>
    <v-container>
        <v-row>
            <v-col cols="12" md="4">
            File input
                <v-file-input label="file input"></v-file-input>
            </v-col>
            <v-col cols="12" md="4">
            Number input
                <v-number-input
                :reverse="false"
                controlVariant="default"
                label="" :hideInput="false" inset="false">
                </v-number-input>
            </v-col>
            <v-col cols="12" md="4">
            Otp input
                <v-otp-input></v-otp-input>
            </v-col>
        </v-row>
    </v-container>
</template>

<script></script>