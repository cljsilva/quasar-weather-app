<template>
  <q-page class="flex flex-center bg-primary">
     <q-card class="" style="width: 300px; height:auto; display: flex; flex-direction: column; align-items: center">

      <q-card-section class="full-width">
        <div class="text-h5">Esqueci minha senha</div>
        <div class="text-caption">Informe seu e-mail cadastrado para recuperar a senha:</div>
      </q-card-section>

      <q-card-section class="q-pt-none">
        <q-input filled v-model="email" label="E-mail" />
      </q-card-section>

      <q-card-actions class="full-width">
        <q-btn no-caps class="q-mx-sm" color="primary" label="Redefinir senha" @click="$router.push({name: 'login'})" style="width: 100%"/>
      </q-card-actions>
    </q-card>

    <q-card class="my-card">
      <q-img src="https://cdn.quasar.dev/img/parallax2.jpg">
        <div class="absolute-bottom text-subtitle2 text-center">
          Title
        </div>
      </q-img>
    </q-card>
  </q-page>
</template>

<script>
export default {
  name: 'PageIndex',
  data () {
    return {
      login: {
        email: ''
      }
    }
  },
  methods: {

  }
}
</script>
