<template>
    <v-card class="mx-auto" max-width="430">
        <v-layout>
           <v-app-bar color="teal-lighten-3" density="prominent">
                <template v-slot:prepend>
                    <v-app-bar-nav-icon></v-app-bar-nav-icon>
                </template>
                <v-app-bar-title class="text-center pa-10">
                I LOVE BBONZI!!!❤️
                </v-app-bar-title>

                <template v-slot:append>
                    <v-btn icon>
                        <v-icon>mdi-dots-vertical</v-icon>
                    </v-btn>
                </template>
            </v-app-bar>

            <v-main>
                <v-container fluid>
                    <v-card
                    class="mb-2"
                    density="compact"
                    prepend-avatar="https://randomuser.me/api/portraits/women/10.jpg"
                    subtitle="난 뽄지를 좋아하지 않는다 for 진희"
                    title="Happy"
                    variant="text"
                    border>
                        <v-img height="128" src="https://picsum.photos/512/128?image=660" cover/>
                        <v-card-text>
                        난 정말 뽄지를 좋아하지 않음
                        </v-card-text>
                        <template v-slot:actions>
                            <v-btn color="primary" variant="text">View More</v-btn>
                            <v-btn color="primary" variant="text">See un Map</v-btn>
                        </template>
                    </v-card>
                </v-container>
            </v-main> 
        </v-layout>
    </v-card>
</template>