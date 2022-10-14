<template>
    <div>
        <button @click="onClickChild(menu.m1.number)">{{menu.m1.number}}. {{menu.m1.desc}}</button>
    </div>
    
</template>

<script>
export default {
    components: {
    
    },
    data() {
        return {
            menu: {
                m1: {
                    number: "1",
                    desc: "Krabben Chips",
                    price: 3.60
                },
                m2: {
                    number: "2",
                    desc: "Vegetarische Minifrühlingsrollen",
                    price: 3.60
                },
                m3: {
                    number: "3",
                    desc: "Gebackenes Hühnerfleisch",
                    price: 3.60
                },
                m4: {
                    number: "4",
                    desc: "Frühlingsrolle",
                    price: 4.80
                },
                mS1: {
                    number: "S1",
                    desc: "Gemischter Salat",
                    price: 4.80
                },
                mS3: {
                    number: "S3",
                    desc: "Gemischter Salat m. Huhn",
                    price: 7.80
                },
                m6: {
                    number: "6",
                    desc: "Nudelsuppe",
                    price: 3.60
                },
                m3: {
                    number: "7",
                    desc: "Peking Gulasch Suppe",
                    price: 4.80
                },
                m4: {
                    number: "8",
                    desc: "Hühnerfleisch Suppe",
                    price: 4.80
                },
                mS1: {
                    number: "8g",
                    desc: "Tom Yam Gung",
                    price: 5.50
                },
                mS3: {
                    number: "8h",
                    desc: "Tom Kah Gai",
                    price: 5.50
                },

                m9: {
                    number: "9",
                    desc: "Chop Seuy",
                    price: 7.20
                },
                m10: {
                    number: "10",
                    desc: "Kung Pau",
                    price: 7.50
                },
                m11: {
                    number: "11",
                    desc: "Gebratene Nudeln",
                    price: 6.90
                },
                m12: {
                    number: "12",
                    desc: "Gebratene Glasnudeln",
                    price: 7.20
                },
                m13: {
                    number: "13",
                    desc: "Gebratener Eierreis",
                    price: 6.90
                },
                m14: {
                    number: "14",
                    desc: "Gebr. Gemüse in Süßsauer Soße",
                    price: 7.20
                },
                m15: {
                    number: "15",
                    desc: "Gebr. Gemüse in Kokos-Curry Soße",
                    price: 7.50
                },
                m15a: {
                    number: "15a",
                    desc: "Tom Yam Gung",
                    price: 7.80
                },
                m19: {
                    number: "19",
                    desc: "Szechuan",
                    price: 7.50
                },

                m20: {
                    number: "20/30",
                    desc: "Gebr. Nudeln/Eierreis m. Huhn",
                    price: 7.80
                },
                m20g: {
                    number: "20g/30g",
                    desc: "Gebr. Nudeln/Eierreis m. geb. Huhn",
                    price: 10.90
                },
                m22: {
                    number: "22/32",
                    desc: "Gebr. Nudeln/Eierreis m. Entenfleisch",
                    price: 10.00
                },
                m23: {
                    number: "23/33",
                    desc: "Gebr. Nudeln/Eierreis m. Garnelen",
                    price: 10.50
                },
                m24: {
                    number: "24/34",
                    desc: "Gebr. Nudeln/Eierreis m. Rind",
                    price: 9.20
                },
                m25: {
                    number: "25/35",
                    desc: "Gebr. Nudeln/Eierreis m. knuspriger Ente",
                    price: 11.80
                },
                m26: {
                    number: "26/36",
                    desc: "Bami Goreng / Nasi Goreng",
                    price: 7.80
                },


                m20b: {
                    number: "20b",
                    desc: "Gebr. Glasnudeln m. Huhn",
                    price: 8.30
                },
                m22b: {
                    number: "22b",
                    desc: "Gebr. Glasnudeln m. Entenfleisch",
                    price: 10.50
                },
                m23b: {
                    number: "23b",
                    desc: "Gebr. Glasnudeln m. Garnelen",
                    price: 11.00
                },
                m24b: {
                    number: "24b",
                    desc: "Gebr. Glasnudeln m. Rind",
                    price: 9.70
                },
                m25b: {
                    number: "25b",
                    desc: "Gebr. Glasnudeln m. knuspriger Ente",
                    price: 7.80
                },

                m40: {
                    number: "40",
                    desc: "Hühnerfleisch Chop Seuy",
                    price: 9.20
                },
                m41: {
                    number: "41",
                    desc: "Hühnerfleisch Kung Pau",
                    price: 9.40
                },
                m42: {
                    number: "42",
                    desc: "Hühnerfleisch Kokos-Curry Soße",
                    price: 9.40
                },
                m42a: {
                    number: "42a",
                    desc: "Hühnerfleisch in rotem Thai-Curry",
                    price: 9.60
                },
                m43: {
                    number: "43",
                    desc: "Gebackenes Hühnerfleisch (6.Stk) u. Süßsauer",
                    price: 8.20
                },
                m43b: {
                    number: "43b",
                    desc: "Nr. 43 + Gemüse",
                    price: 11.40
                },
                m44: {
                    number: "44",
                    desc: "Gebackenes Hühnerfleisch (6.Stk) u. Erdnuss",
                    price: 9.60
                },
                m44b: {
                    number: "44b",
                    desc: "Nr. 44 + Gemüse",
                    price: 11.40
                },
                m46: {
                    number: "46",
                    desc: "Hühnerfleisch Süßsauer",
                    price: 9.20
                },
                m47: {
                    number: "47",
                    desc: "Hühnerfleisch Soja Soße",
                    price: 9.20
                },
                m49: {
                    number: "49",
                    desc: "Hühnerfleisch Szechuan",
                    price: 9.40
                }

            }

        }
    },
    methods: {
        onClickChild(value) {
            this.$emit('clickedKey', value);
        },
    }


}
</script>


