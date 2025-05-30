<template>
    <v-card class="mx-auto" max-width="430">
        <v-layout>
            <v-app-bar color="info" density="prominent">
                <template v-slot:prepend>
                    <v-app-bar-nav-icon></v-app-bar-nav-icon>
                </template>
                <v-app-bar-title>HAYAN ✨</v-app-bar-title>

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
                    prepend-avatar="http://randomuser.me/api/portraits/women/10.jpg"
                    subtitle="우리집 침대 위에서 우래기들이랑 누워있고 싶당"
                    title="Sweet my Home"
                    variant="text"
                    border
                    >
                    <v-img height="128" src="http://picsum.photos/512/128?image=660" cover></v-img>
                    <v-card-text>
                        집에 갈래용
                    </v-card-text>
                    <template v-slot:actions>
                        <v-btn color="primary" variant="text">view more</v-btn>
                        <v-btn color="primary" variant="text">Click me</v-btn>
                    </template>
                    </v-card>
                </v-container>
            </v-main>
        </v-layout>
    </v-card>
</template>