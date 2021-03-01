<template>
  <v-app>
    <v-main>
      <v-container>
        <v-row class="text-center"
          ><v-col cols="12"><h1>Logicky Soudržná Republika</h1></v-col></v-row
        >

        <v-row class="text-center"
          ><v-col cols="12"
            ><h2 class="grey--text">Formulář žádosti o občanství</h2></v-col
          ></v-row
        >
        <v-row class="text-center"
          ><v-col cols="3" offset="3"
            ><v-text-field label="Jméno"></v-text-field></v-col
          ><v-col cols="3"><v-text-field label="Příjmení"></v-text-field></v-col
        ></v-row>
        <v-row class="text-center"
          ><v-col cols="3" offset="3"
            ><v-text-field
              label="Datum narození"
              placeholder="01.01.1901"
            ></v-text-field></v-col
          ><v-col cols="3"
            ><v-text-field label="Místo narození"></v-text-field></v-col
        ></v-row>
        <v-row
          ><v-col cols="1" offset="3"><v-label>Pohlaví</v-label></v-col
          ><v-col cols="5"
            ><v-slider
              prepend-icon="mdi-cat"
              append-icon="mdi-dog"
              value="50"
            ></v-slider></v-col
        ></v-row>
        <hr />
        <p></p>
        <v-row
          ><v-col cols="5" offset="3"
            ><h3>Povinné požadavky na občanství</h3></v-col
          ></v-row
        >
        <v-row
          ><v-col cols="5" offset="4"
            ><v-checkbox
              label="Zaručuji, že mluvím nativně latinsky"
            ></v-checkbox></v-col
        ></v-row>
        <v-row
          ><v-col cols="5" offset="4"
            ><v-checkbox
              label="Vážně přísahám, že jsem na tom dobře "
            ></v-checkbox></v-col
        ></v-row>
        <v-row
          ><v-col offset="4"
            ><b> Zvažte následující větu: „nikdo tam není“. </b>Kolik je tam
            lidí?
          </v-col></v-row
        >
        <v-row>
          <v-col cols="5" offset="5">
            <v-radio-group>
              <v-radio label="nikdo"></v-radio>
              <v-radio label="někdo"></v-radio>
            </v-radio-group>
          </v-col>
        </v-row>
        <v-row>
          <v-col cols="12" class="text-center"
            ><v-btn color="red" align="center" justify="center"
              >Odeslat</v-btn
            ></v-col
          >
        </v-row>
      </v-container>
    </v-main>
  </v-app>
</template>

<script>
export default {
  name: "App",

  data: () => ({
    birthdate: "",
  }),
};
</script>
