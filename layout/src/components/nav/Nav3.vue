<template>
    <v-card class="mx-auto" color="gray-light-3" max-width="768">
        <v-layout>
            <v-app-bar color="teal-darken-4" image="https://picsum.photos/1920/1080?random"> <!-- 랜덤 이미지 -->
                <template v-slot:image> <!-- 글씨 보이게 설정 -->
                    <v-img gradient="to top right, rgba(19, 84, 122, .8), rgba(128, 208, 190, .8)"></v-img>
                </template>

                <template v-slot:prepend> <!-- 햄버거 아이콘 -->
                    <v-app-bar-nav-icon></v-app-bar-nav-icon>
                </template>

                <v-app-bar-title>HAYAN</v-app-bar-title>

                <v-btn icon> <!-- 돋보기 버튼 -->
                    <v-icon>mdi-magnify</v-icon>
                </v-btn>

                <v-btn icon> <!-- 좋아요 버튼 -->
                    <v-icon>mdi-heart</v-icon>
                </v-btn>

                <v-btn icon> <!-- 더보기 버튼 -->
                    <v-icon>mdi-dots-vertical</v-icon>
                </v-btn>
            </v-app-bar>

            <v-main>
                <v-container fluid>
                    <v-row dense> <!-- 간격 줄여서 더 촘촘하게 -->
                        <v-col
                        v-for="n in 4"
                        :key="n"
                        cols="12">
                        <v-card
                        :subtitle="`Subtitle for Content ${n}`"
                        :title="`Content ${n}`"
                        text="lorem1">

                        </v-card>
                        </v-col>
                    </v-row>
                </v-container>
            </v-main>
        </v-layout>
    </v-card>
</template>