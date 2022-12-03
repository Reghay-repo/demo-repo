<template>
  <v-card
      flat
    class="mx-auto"
    height="auto"
    width="auto"
  >
    <br>
    <v-list >
      <v-list-item prepend-icon="mdi-view-dashboard-outline" title="Dashboard"></v-list-item>
      <br>
      <ListItem  :items="manage"/>
      <ListItem  :items="client"/>
      <ListItem  :items="droit"/>
      <ListItem  :items="Partenaires"/>
      <ListItem  :items="ressources_humaines"/>
      <ListItem  :items="comptable"/>
      <ListItem  :items="reglages"/>
    </v-list>
  </v-card>
</template>

<script setup>
const manage = {
  title:'manage',
  list:[
    'ville',
    'complexe',
    'residence',
    'terrain',
    'villa',
    'immeuble',
  ]
}
const client = {
  title:'client',
  list:[
    'Syndic',
    'Copropriétaires',
    'Reçus',
    'Factures',
    'Revenus et dépenses',
    'Bénéfices/pertes',
    'comptes bancaires',
    'Comptabilité',
    'Assemblée générale',
    'Assistance',
    'Résoudre les conflits',
    'immeublez',
  ]
}

const droit = {
  title:'Droit et justice',
  list:[
    'Procédure judiciaires',
    'Suivi judiciaire',
  ]
}
const Partenaires = {
  title:'Partenaires et fournisseurs',
  list:[
    'Partenaires commerciaux ',
    'Partenaires professionnels ',
    'Fournisseurs',
  ]
}

const ressources_humaines = {
  title:'Gestion des ressources humaines',
  list:[
    'Départements',
    'Employés',
    'Présence',
    'Salaires mensuels',
    'Vacances',
  ]
}
const comptable = {
  title:'Société comptable et financière',
  list:[
    'Revenus',
    'Dépenses',
    'Bénéfices/pertes',
    'Compte bancaire',
    'Comptabilité',
    'Taxes et permis',
  ]
}
const reglages = {
  title:'réglages',
  list:[
    'Utilisateurs et autorisations',
    'Langues',
    'Réglage des SMS',
    'Configuration de la messagerie',
    'Base de données de sauvegarde',
    'Devise',
  ]
}


</script>

<style scoped>

</style>