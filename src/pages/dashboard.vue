<script setup>
import AnalyticsCongratulations from '@/views/dashboard/AnalyticsCongratulations.vue'
import AnalyticsFinanceTabs from '@/views/dashboard/AnalyticsFinanceTab.vue'
import AnalyticsOrderStatistics from '@/views/dashboard/AnalyticsOrderStatistics.vue'
import AnalyticsProfitReport from '@/views/dashboard/AnalyticsProfitReport.vue'
import AnalyticsTotalRevenue from '@/views/dashboard/AnalyticsTotalRevenue.vue'
import AnalyticsTransactions from '@/views/dashboard/AnalyticsTransactions.vue'
import DemoSimpleTableBasics from '@/views/pages/tables/DemoSimpleTableBasics.vue'

// 👉 Images
import chart from '@images/cards/chart-success.png'
import card from '@images/cards/credit-card-primary.png'
import paypal from '@images/cards/paypal-error.png'
import wallet from '@images/cards/wallet-info.png'
</script>

<template>
  <VRow>
    <!-- 👉 Congratulations -->
    <VCol
      cols="12"
      md="8"
    >
      <AnalyticsCongratulations />
    </VCol>

    <VCol
      cols="12"
      sm="4"
    >
      <VRow>
        <!-- 👉 Profit -->
        <VCol
          cols="12"
          md="6"
        >
          <CardStatisticsVertical
            v-bind="{
              title: 'Profit',
              image: chart,
              stats: '$873,401',
              change: 137.20,
            }"
          />
        </VCol>

        <!-- 👉 Sales -->
        <VCol
          cols="12"
          md="6"
        >
          <CardStatisticsVertical
            v-bind="{
              title: 'Sales',
              image: wallet,
              stats: '$1.26M',
              change: 28.42,
            }"
          />
        </VCol>
      </VRow>
    </VCol>

    <!-- 👉 Total Revenue -->
    <VCol
      cols="12"
      md="8"
      order="3"
      order-md="2"
    >
      <AnalyticsTotalRevenue />
    </VCol>

    <VCol
      cols="12"
      sm="8"
      md="4"
      order="3"
      order-md="2"
    >
      <VRow>
        <!-- 👉 Payments -->
        <VCol
          cols="12"
          sm="6"
        >
          <CardStatisticsVertical
            v-bind=" {
              title: 'Payments',
              image: paypal,
              stats: '$120.9K',
              change: 14.82,
            }"
          />
        </VCol>

        <!-- 👉 Revenue -->
        <VCol
          cols="12"
          sm="6"
        >
          <CardStatisticsVertical
            v-bind="{
              title: 'Transactions',
              image: card,
              stats: '$140.8K',
              change: 28.14,
            }"
          />
        </VCol>
      </VRow>

      <VRow>
        <!-- 👉 Profit Report -->
        <VCol
          cols="12"
          sm="12"
        >
          <AnalyticsProfitReport />
        </VCol>
      </VRow>
    </VCol>

    <!-- 👉 Order Statistics -->
    <!--
    <VCol
      cols="12"
      md="4"
      sm="6"
      order="4"
    >
      <AnalyticsOrderStatistics />
    </VCol>
    -->

    <!-- 👉 Tabs chart -->
    <!--
    <VCol
      cols="12"
      md="4"
      sm="6"
      order="4"
    >
      <AnalyticsFinanceTabs />
    </VCol>
    -->

    <!-- 👉 Transactions -->
    <!--
    <VCol
      cols="12"
      md="4"
      sm="6"
      order="4"
    >
      <AnalyticsTransactions />
    </VCol>
    -->
  </VRow>

  <VRow>
      <!-- 👉 Orders Table -->
      <VCol cols="12" order="5"> 
        <VCard title="Latest Orders">
          <DemoSimpleTableBasics />
        </VCard>
      </VCol>
    </VRow>

</template>
