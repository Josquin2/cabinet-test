<script setup lang="ts">
import type { link } from '@/types/Link'

const links: Array<link> = [
  {
    img: 'links/dashboard.png',
    title: 'Dashboard'
  },
  {
    img: 'links/transactions.png',
    title: 'Transactions'
  },
  {
    img: 'links/accounts.png',
    title: 'Accounts'
  },
  {
    img: 'links/investments.png',
    title: 'Investments'
  },
  {
    img: 'links/credit-cards.png',
    title: 'Credit Cards'
  },
  {
    img: 'links/loans.png',
    title: 'Loans'
  },
  {
    img: 'links/services.png',
    title: 'Services'
  },
  {
    img: 'links/my-privileges.png',
    title: 'My Privileges'
  },
  {
    img: 'links/setting.png',
    title: 'Setting'
  }
]
</script>

<template>
  <nav class="navigation-bar">
    <div class="main-logo">
      <img src="/icons/main-logo.png" alt="" />
    </div>
    <div class="nav-links">
      <button
        class="one-link"
        v-for="(link, index) in links"
        :key="index"
        :class="{ 'current-link': link?.title == 'Setting' }"
      >
        <img :src="link?.img" alt="" />
        <p>{{ link?.title }}</p>
      </button>
    </div>
  </nav>
</template>

<style lang="scss">
@media only screen and (max-width: 950px) {
  .navigation-bar {
    width: 0;
  }
}
</style>
