    <template>
              <chart :chart-data="datacollection"></chart>
    </template>
    <script>
    import Chart from "./../chart.js";
    export default {
      components: {
        Chart
      },
      data() {
        return {
          datacollection: null
        };
      },
      mounted() {
        this.fillData();
      },
      methods: {
        fillData() {
          this.datacollection = {
            labels: [
              "January",
              "February",
              "March",
              "April",
              "May",
              "June",
              "July",
              "August",
              "September",
              "October",
              "November",
              "December"
            ],
            datasets: [
              {
                label: "Active Users",
                borderColor: "#f96332",
                pointBorderColor: "#FFF",
                pointBackgroundColor: "#f96332",
                pointBorderWidth: 2,
                pointHoverRadius: 4,
                pointHoverBorderWidth: 1,
                pointRadius: 4,
                fill: true,
                backgroundColor: "#f7b733",
                borderWidth: 2,
                data: [70, 20, 12, 39, 100, 40, 95, 80, 80, 20, 12, 101]
              },
              {
                label: "Monthly incomes",
                backgroundColor: "#A5CC82",
                data: [34, 408, 188, 190, 58, 200, 190, 400, 164, 254, 290, 201]
              }
            ]
          };
        },
      }
    };
    </script>
    <style>
    </style>