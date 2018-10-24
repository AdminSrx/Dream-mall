<template>
  <div>
    <v-content>
      <v-container fluid fill-height>
        <v-layout align-center justify-center>
          <v-flex xs12 sm8 md4>
            <v-card class="elevation-12">
              <v-toolbar dark color="primary">
                <v-toolbar-title>登录</v-toolbar-title>
                <v-spacer></v-spacer>
                <v-tooltip right>
                  <span>Codepen</span>
                </v-tooltip>
              </v-toolbar>
              <v-card-text>
                <v-form>
                  <v-text-field prepend-icon="person" name="login" label="Login" type="text"></v-text-field>
                  <v-text-field id="password" prepend-icon="lock" name="password" label="Password" type="password"></v-text-field>
                </v-form>
              </v-card-text>
              <v-card-actions>
                <v-spacer></v-spacer>
                <v-btn color="primary" class="lighten-5">Login</v-btn>
              </v-card-actions>
            </v-card>
          </v-flex>
        </v-layout>
      </v-container>
    </v-content>
    <div>
      <v-container grid-list-md text-xs-center>
        <v-layout row wrap>
          <v-flex xs12>
            <v-card dark color="primary">
              <v-card-text class="px-0">12</v-card-text>
            </v-card>
          </v-flex>
          <v-flex v-for="i in 2" :key="`6${i}`" xs6>
            <v-card dark color="secondary">
              <v-card-text class="px-0">6</v-card-text>
            </v-card>
          </v-flex>
          <v-flex v-for="i in 3" :key="`4${i}`" xs4>
            <v-card dark color="primary">
              <v-card-text class="px-0">4</v-card-text>
            </v-card>
          </v-flex>
          <v-flex v-for="i in 4" :key="`3${i}`" xs3>
            <v-card dark color="secondary">
              <v-card-text class="px-0">3</v-card-text>
            </v-card>
          </v-flex>
          <v-flex v-for="i in 6" :key="`2${i}`" xs2>
            <v-card dark color="primary">
              <v-card-text class="px-0">2</v-card-text>
            </v-card>
          </v-flex>
          <v-flex v-for="i in 12" :key="`1${i}`" xs1>
            <v-card dark color="secondary">
              <v-card-text class="px-0">1</v-card-text>
            </v-card>
          </v-flex>
        </v-layout>
      </v-container>
    </div>
  </div>
</template>

<script>
  export default {
    data: () => ({
      drawer: null
    }),
    props: {
      source: String
    }
  }
</script>

<style scoped>

</style>

