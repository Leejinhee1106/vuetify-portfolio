<template>
    <v-container>
        <v-row>
            <v-col cols="12" md="4">
                <h1>One</h1>
                <v-breadcrumbs bg-color="warning" :items="['what','happen','?']"/>
            </v-col>

            <v-col cols="12" md="6">
                <h1>Two</h1>
                  <div>
                    <v-breadcrumbs
                      :items="items"
                      divider="-"
                    ></v-breadcrumbs>

                    <v-breadcrumbs
                      :items="items"
                      divider="."
                    ></v-breadcrumbs>
                  </div>
            </v-col>
        </v-row>
    </v-container>
</template>

<script setup>
  const items = [
    {
      title: 'Dashboard',
      disabled: false,
      href: 'breadcrumbs_dashboard',
    },
    {
      title: 'Link 1',
      disabled: false,
      href: 'breadcrumbs_link_1',
    },
    {
      title: 'Link 2',
      disabled: true,
      href: 'breadcrumbs_link_2',
    },
  ]
</script>