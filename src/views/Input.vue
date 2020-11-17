<template>
    <v-container fluid>
        <v-row>
            <v-col cols="6">
                <v-card color="#B2DFDB"> 
                    <v-form ref="form" v-model="valid" lazy-validation>
                        <v-text-field v-model="name" :counter="10" :rules="nameRules" label="Your Name" required>

                        </v-text-field>
                        <v-text-field v-model="name" :counter="30" :rules="nameRules" label="Your Phone Number"
                            required>
                        </v-text-field>
                        <v-menu ref="menu" v-model="menu" :close-on-content-click="false" transition="scale-transition"
                            offset-y min-width="290px">
                            <template v-slot:activator="{ on, attrs }">
                                <v-text-field v-model="date" label="Booking date" prepend-icon="mdi-calendar" readonly
                                    v-bind="attrs" v-on="on"></v-text-field>
                            </template>
                            <v-date-picker ref="picker" v-model="date" :max="new Date().toISOString().substr(0, 10)"
                                min="1950-01-01" @change="save"></v-date-picker>
                        </v-menu>
                        <v-btn color="#004D40" text--white>
                            Send
                        </v-btn>
                    </v-form>
                </v-card>
            </v-col>
        </v-row>
    </v-container>
</template>
<script>
    export default {
        data: () => ({
            date: null,
            menu: false,
        }),
        watch: {
            menu(val) {
                val && setTimeout(() => (this.$refs.picker.activePicker = 'YEAR'))
            },
        },
        methods: {
            save(date) {
                this.$refs.menu.save(date)
            },
        },
    }
</script>