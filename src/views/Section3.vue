<template>
    <div>
        <!-- section 3 -->
        <section>
            <v-row>
                <v-col cols='12'>
                    <div class="video-player">
                        <video class="video" ref="video">
                            <source :src="require(`@/assets/videoplayback.mp4`)" type="video/mp4">
                        </video>
                    </div>
                </v-col>
            </v-row>
        </section>
    </div>
</template>

<script>
    export default {
        components: {},
        data: () => ({
            //
        }),
        computed: {
            videoElement() {
                return this.$refs.video;
            }
        },
        created(){
            this.videoElement
        }
    }
</script>