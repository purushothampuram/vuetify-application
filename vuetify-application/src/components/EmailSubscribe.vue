<template>
  <v-card color="grey lighten-3">
  <v-container grid-list>
    <v-layout row wrap>
      <v-flex md12 class="heading">
        <v-card class="email-card">
          <v-card-title primary-title class="card-title">
            <div>
              <h1>Would You Like Us To Contact You with Special Offers and Business News?</h1>
            </div>
          </v-card-title>
        </v-card>
      </v-flex>
    </v-layout>
    <v-layout row wrap class="contact-elements">
      <v-flex xs2>
      </v-flex>
        <v-flex xs12 md4 class="contact-email">
          <v-subheader class="subHeading"><h3>Email Address</h3></v-subheader>
        <v-text-field class="field-spaces"
          v-model="email"
          label="Your E-mail"
        ></v-text-field>
      </v-flex>
        <v-flex xs12 md4 class="contact-industry">
          <v-subheader class="subHeading"><h3>Select your Industry</h3></v-subheader>
          <v-select class="field-spaces"
            label="Select"
            single-line
          ></v-select>
        </v-flex>
    </v-layout>
    <v-layout row justify-center>
      <v-flex xs2>
        <button class="submit">
          <img src="../assets/Button3.png" />
        </button>
      </v-flex>
    </v-layout>
  </v-container>
    </v-card>
</template>

<script>
export default{
  data: () => ({
    valid: true,
    email: ''
  })
}
</script>
<style scoped>
  .contact-heading{
  }
  .contact-elements{
    .margin-top:40px;
  }
  .contact-email{
    margin-right:40px;
  }
  .contact-industry{
    margin-left:40px;
  }
.submit{
  height: 50px;
  width: 180px;
  margin-bottom: 20px;
  margin-top: 40px;
  }
  .heading{
    padding: 30px;
  }
  .email-card{
    margin-left:70px;
    margin-right:70px;
  }
  .field-spaces{
    width: 434px;
  }
  .subHeading{
    margin-bottom: 0px!important;
    font-weight: 400;
    padding:0px;
    color: #000000;
  }
  .card-title{
    padding-top: 15px;
    padding-bottom: 15px;
    margin-left: 40px;
    margin-right: 40px;
  }
</style>
