<template>
  <v-stepper
    v-model="e6"
    vertical
  >
    <v-stepper-step
      :complete="e6 > 1"
      step="1"
    >
      Step 1 : Site Incident
    </v-stepper-step>

    <v-stepper-content step="1">
      <v-card
        color="grey lighten-1"
        class="mb-12"
        height="200px"
      ></v-card>
      <v-btn
        color="primary"
        @click="e6 = 2"
      >Continue</v-btn>
      <v-btn text>Cancel</v-btn>
    </v-stepper-content>

    <v-stepper-step
      :complete="e6 > 2"
      step="2"
    >
      Step 2 : SysOps Incident
    </v-stepper-step>

    <v-stepper-content step="2">
      <v-card
        color="grey lighten-1"
        class="mb-12"
        height="200px"
      ></v-card>
      <v-btn
        color="primary"
        @click="e6 = 3"
      >Continue</v-btn>
      <v-btn text>Cancel</v-btn>
    </v-stepper-content>

    <v-stepper-step
      :complete="e6 > 3"
      step="3"
    >
      Step 3 : SCTASKS
    </v-stepper-step>

    <v-stepper-content step="3">
      <v-card
        color="grey lighten-1"
        class="mb-12"
        height="200px"
      ></v-card>
      <v-btn
        color="primary"
        @click="e6 = 4"
      >Continue</v-btn>
      <v-btn text>Cancel</v-btn>
    </v-stepper-content>

    <v-stepper-step
      :complete="e6 > 4"
      step="4"
    >
      Step 4 : Additional Instructions and Other Information
    </v-stepper-step>
    <v-stepper-content step="4">
      <v-card
        color="grey lighten-1"
        class="mb-12"
        height="200px"
      ></v-card>
      <v-btn
        color="primary"
        @click="e6 = 5"
      >Continue</v-btn>
      <v-btn text>Cancel</v-btn>
    </v-stepper-content>
    <v-stepper-step
      :complete="e6 > 5"
      step="5"
    >
      Step 5 : Display Diagram
    </v-stepper-step>
    <v-stepper-content step="5">
      <v-card
        color="grey lighten-1"
        class="mb-12"
        height="200px"
      ></v-card>
      <v-btn
        color="primary"
        @click="e6 = 6"
      >Continue</v-btn>
      <v-btn text>Cancel</v-btn>
    </v-stepper-content>
    <v-stepper-step
      :complete="e6 > 6"
      step="6"
    >
      Step 6 : Review Report and Send Email
    </v-stepper-step>
    <v-stepper-content step="6">
      <v-card
        color="grey lighten-1"
        class="mb-12"
        height="200px"
      ></v-card>
      <v-btn
        color="primary"
        @click="e6 = 7"
      >Send Email</v-btn>
    </v-stepper-content>
  </v-stepper>
</template>

<script>
export default {
  data() {
    return {
      e6: 1,
    }
  },
}
</script>