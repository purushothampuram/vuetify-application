<template>
  <div class ="subscribe">
  <v-container grid-list>
    <v-layout row wrap>
      <v-flex md12 class="heading">
        <div class="email-card">
              <h2 class="card-title">Would You Like Us To Contact You with Special Offers and Business News?</h2>
        </div>
      </v-flex>
    </v-layout>
    <v-layout row wrap class="contact-elements">
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
          <img class="submit" src='../assets/Button3.png' />
      </v-flex>
    </v-layout>
  </v-container>
    </div>
</template>

<script>
export default{
  data: () => ({
    valid: true,
    email: ''
  })
}
</script>
<style>
  .contact-elements{
    margin-top:40px;
  }
  .contact-email{
    margin-right:40px;
    margin-left:60px;
  }
  .contact-industry{
    margin-left:40px;
    padding-left: 40px;
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
    margin-left: 220px;
    margin-right: 220px;
    background-color: white;
  }
  .field-spaces{
    width: 434px;
  }
  .subheader{
    margin-bottom: 0px!important;
    font-weight: 400;
    font-size: 20px;
    padding: 0px;
    font-family: 'Open Sans Bold';
  }
  .card-title{
    padding-top: 15px;
    padding-bottom: 15px;
    margin-left: 40px;
    margin-right: 40px;
    font-family: 'Open Sans Bold';
    font-size: 32px;
  }
  .subscribe{
    background-color: #EEEEEE;
    margin-left: 20px;
    margin-right: 20px;
  }
</style>
