<template>
  <header id="header">
    <v-navigation-drawer app v-model="drawer">
      <v-container>
        <v-list-item>
          <v-list-item-content>
            <v-list-item-title class="title">
              メニュー
            </v-list-item-title>
          </v-list-item-content>
        </v-list-item>
        <v-divider></v-divider>
        <v-list dense nav>
          <v-list-item v-for="nav_list in nav_lists" :key="nav_list.name">
            <v-list-item-icon>
              <v-icon>{{ nav_list.icon }}</v-icon>
            </v-list-item-icon>
            <v-list-item-content>
              <v-list-item-title>{{ nav_list.name }}</v-list-item-title>
            </v-list-item-content>
          </v-list-item>
        </v-list>
      </v-container>
    </v-navigation-drawer>
    <v-app-bar color="#F9A825" dark app>
      <v-app-bar-nav-icon @click="drawer=!drawer"></v-app-bar-nav-icon>
      <v-toolbar-title>wakeco</v-toolbar-title>
      <v-spacer></v-spacer>
      <v-btn outlined>新規登録</v-btn>
      <v-btn outlined class="ml-2">ログイン</v-btn>
    </v-app-bar>
  </header>
</template>

<script>
  export default {
    name: 'Header',
    data: function () {
      return {
        drawer: null,
        nav_lists:[
          {name: 'プロフィール',icon: 'mdi-account'},
          {name: 'コミュニティ',icon: 'mdi-account-group'},
          {name: '購入履歴',icon: 'mdi-cart-arrow-down'},
          {name: '出品履歴',icon: 'mdi-cart-arrow-up'},
          {name: '設定',icon: 'mdi-account-cog'},
          {name: 'アカウント',icon: 'mdi-account-cog'},
        ]
      }
    }
  }
</script>
