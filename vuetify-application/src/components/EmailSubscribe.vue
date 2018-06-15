<template>
  <div class ="subscribe">
  <v-container grid-list>
    <v-layout row wrap>
      <v-flex md12 class="heading">
        <div class="email-card">
              <h3 class="card-title">Would You Like Us To Contact You with Special Offers and Business News?</h3>
        </div>
      </v-flex>
    </v-layout>
    <v-layout row wrap class="contact-elements">
        <v-flex xs12 md4 class="contact-email">
          <v-subheader class="subHeading"><h4>Email Address</h4></v-subheader>
        <v-text-field class="field-spaces"
          v-model="email"
          label="Your E-mail"
        ></v-text-field>
      </v-flex>
        <v-flex xs12 md4 class="contact-industry">
          <v-subheader class="subHeading"><h4>Select your Industry</h4></v-subheader>
          <v-select class="field-spaces"
                    :items="industries"
                    v-model="industry"
                    label="Select"
                    single-line
          ></v-select>
        </v-flex>
    </v-layout>
    <v-layout row justify-center>
      <v-flex xs2>
          <img class="submit" src='../assets/Button3.png' @click.stop="dialog3 = true"/>
      </v-flex>
      <v-dialog v-model="dialog3" max-width="500px">
        <v-card>
          <v-card-title>
            <span>Success</span>
          </v-card-title>
          <v-card-text>
            Subscribed Successfully!
          </v-card-text>
          <v-card-actions>
            <v-btn color="primary" flat @click.stop="dialog3=false">Close</v-btn>
          </v-card-actions>
        </v-card>
      </v-dialog>
    </v-layout>
  </v-container>
    </div>
</template>

<script>
export default{
  data: () => ({
    email: '',
    industries: [
      'Industry 1', 'Industry 2', 'Industry 3', 'Industry 4', 'Industry 5'
    ],
    industry: null,
    dialog3: false
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
  text-shadow: 0px 1px 2px;
  outline: 1px #333333;
  font-family: 'Open Sans Bold';
  color: #333333;
  font-size: 21px;
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
  .subHeading{
    margin-bottom: 0px!important;
    padding: 0px;
    font-family: 'Open Sans Bold';
  }
  h3{
    font-size: 32px;
    font-family: 'Open Sans ExtraBold';
    color:#333333;
  }
  h4{
    font-family: 'Open Sans ExtraBold';
    font-size: 28px;
    color: #333333;
  }
  .card-title{
    padding-top: 15px;
    padding-bottom: 15px;
    margin-left: 40px;
    margin-right: 40px;
  }
  .subscribe{
    background-color: #EEEEEE;
    margin-left: 20px;
    margin-right: 20px;
  }
</style>
