<script setup>
const orders = [
  {
    orderNumber: 28456,
    customerName: 'William Martinez',
    orderDate: '2024-04-10',
    paymentTotal: '$1800',
    paymentStatus: 'Pending',
    fulfillmentStatus: 'Completed',
    customerEmail: 'williammartinez39@gmail.com'
  },
  {
    orderNumber: 28457,
    customerName: 'Sarah Wilson',
    orderDate: '2024-04-02',
    paymentTotal: '$900',
    paymentStatus: 'Completed',
    fulfillmentStatus: 'Pending',
    customerEmail: 'sarahwilson92@gmail.com'
  },
  {
    orderNumber: 28458,
    customerName: 'Charles Williams',
    orderDate: '2024-04-12',
    paymentTotal: '$3600',
    paymentStatus: 'Pending',
    fulfillmentStatus: 'Completed',
    customerEmail: 'charleswilliams30@gmail.com'
  },
    {
    orderNumber: 28459,
    customerName: 'Sarah Gonzalez',
    orderDate: '2024-04-07',
    paymentTotal: '$900',
    paymentStatus: 'Completed',
    fulfillmentStatus: 'Pending',
    customerEmail: 'sarahgonzalez16@gmail.com'
  },
  {
    orderNumber: 28460,
    customerName: 'William Davis',
    orderDate: '2024-04-10',
    paymentTotal: '$3600',
    paymentStatus: 'Completed',
    fulfillmentStatus: 'Pending',
    customerEmail: 'williamdavis32@gmail.com'
  },
  {
    orderNumber: 28461,
    customerName: 'Robert Johnson',
    orderDate: '2024-04-01',
    paymentTotal: '$900',
    paymentStatus: 'Pending',
    fulfillmentStatus: 'Pending',
    customerEmail: 'robertjohnson44@gmail.com'
  },
  {
    orderNumber: 28462,
    customerName: 'David Lopez',
    orderDate: '2024-04-03',
    paymentTotal: '$1800',
    paymentStatus: 'Completed',
    fulfillmentStatus: 'Completed',
    customerEmail: 'davidlopez54@gmail.com'
  },
  {
    orderNumber: 28463,
    customerName: 'John Smith',
    orderDate: '2024-04-14',
    paymentTotal: '$1800',
    paymentStatus: 'Pending',
    fulfillmentStatus: 'Completed',
    customerEmail: 'johnsmith83@gmail.com'
  },
  {
    orderNumber: 28464,
    customerName: 'John Brown',
    orderDate: '2024-04-09',
    paymentTotal: '$1800',
    paymentStatus: 'Completed',
    fulfillmentStatus: 'Pending',
    customerEmail: 'johnbrown72@gmail.com'
  },
  {
    orderNumber: 28465,
    customerName: 'Lisa Taylor',
    orderDate: '2024-04-11',
    paymentTotal: '$900',
    paymentStatus: 'Completed',
    fulfillmentStatus: 'Completed',
    customerEmail: 'lisataylor33@gmail.com'
  },
  {
    orderNumber: 28466,
    customerName: 'Paul Jones',
    orderDate: '2024-04-10',
    paymentTotal: '$2700',
    paymentStatus: 'Pending',
    fulfillmentStatus: 'Pending',
    customerEmail: 'pauljones58@gmail.com'
  },
  {
    orderNumber: 28467,
    customerName: 'Laura Wilson',
    orderDate: '2024-04-15',
    paymentTotal: '$1800',
    paymentStatus: 'Pending',
    fulfillmentStatus: 'Completed',
    customerEmail: 'laurawilson43@gmail.com'
  },
  {
    orderNumber: 28468,
    customerName: 'John Martinez',
    orderDate: '2024-04-04',
    paymentTotal: '$2700',
    paymentStatus: 'Completed',
    fulfillmentStatus: 'Completed',
    customerEmail: 'johnmartinez75@gmail.com'
  },
  {
    orderNumber: 28469,
    customerName: 'Joseph Garcia',
    orderDate: '2024-04-14',
    paymentTotal: '$2700',
    paymentStatus: 'Pending',
    fulfillmentStatus: 'Completed',
    customerEmail: 'josephgarcia95@gmail.com'
  },
  {
    orderNumber: 28470,
    customerName: 'Robert Rodriguez',
    orderDate: '2024-04-08',
    paymentTotal: '$2700',
    paymentStatus: 'Completed',
    fulfillmentStatus: 'Pending',
    customerEmail: 'robertrodriguez90@gmail.com'
  },
  {
    orderNumber: 28471,
    customerName: 'Thomas Rodriguez',
    orderDate: '2024-04-12',
    paymentTotal: '$1800',
    paymentStatus: 'Completed',
    fulfillmentStatus: 'Completed',
    customerEmail: 'thomasrodriguez69@gmail.com'
  },
  {
    orderNumber: 28472,
    customerName: 'Michael Rodriguez',
    orderDate: '2024-04-02',
    paymentTotal: '$900',
    paymentStatus: 'Pending',
    fulfillmentStatus: 'Pending',
    customerEmail: 'michaelrodriguez81@gmail.com'
  },
  {
    orderNumber: 28473,
    customerName: 'Charles Jackson',
    orderDate: '2024-04-05',
    paymentTotal: '$900',
    paymentStatus: 'Pending',
    fulfillmentStatus: 'Pending',
    customerEmail: 'charlesjackson55@gmail.com'
  },
  {
    orderNumber: 28474,
    customerName: 'David Miller',
    orderDate: '2024-04-15',
    paymentTotal: '$3600',
    paymentStatus: 'Completed',
    fulfillmentStatus: 'Pending',
    customerEmail: 'davidmiller51@gmail.com'
  },
  {
    orderNumber: 28475,
    customerName: 'William Anderson',
    orderDate: '2024-04-02',
    paymentTotal: '$2700',
    paymentStatus: 'Pending',
    fulfillmentStatus: 'Completed',
    customerEmail: 'williamanderson27@gmail.com'
  }
  // ... Add the rest of the orders in the same format
];
</script>


<template>
  <VTable>
    <thead>
      <tr>
        <th>Order Number</th>
        <th>Customer Name</th>
        <th>Order Date</th>
        <th>Payment Total</th>
        <th>Payment Status</th>
        <th>Fulfillment Status</th>
        <th>Customer Email</th>
      </tr>
    </thead>
    <tbody>
      <tr v-for="order in orders" :key="order.orderNumber">
        <td>{{ order.orderNumber }}</td>
        <td>{{ order.customerName }}</td>
        <td>{{ order.orderDate }}</td>
        <td>{{ order.paymentTotal }}</td>
        <td>{{ order.paymentStatus }}</td>
        <td>{{ order.fulfillmentStatus }}</td>
        <td>{{ order.customerEmail }}</td>
      </tr>
    </tbody>
  </VTable>
</template>
