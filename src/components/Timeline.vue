<template>
  <v-simple-table dense>
    <template v-slot:default>
      <thead>
        <tr>
          <th class="text-left">SUBJECT CODE</th>
          <th class="text-left">SUBJECT NAME</th>
          <th class="text-left">STATUS</th>
        </tr>
      </thead>
      <tbody>
        <tr v-for="item in subject" :key="item.code">
          <td>{{ item.code }}</td>
          <td>{{ item.name }}</td>
          <td>
            <span :class="[item.statusClass]">{{ item.status }}</span>
          </td>
        </tr>
      </tbody>
    </template>
  </v-simple-table>
</template>

<script>
export default {
  data() {
    return {
      subject: [
        {
          name: "Military training",
          code: "GDQP",
          statusClass: "passed",
          status: "Passed",
          reason: "",
        },
        {
          name: "Vovinam 2",
          code: "VOV124",
          statusClass: "passed",
          status: "Passed",
          reason: "",
        },
        {
          name: "Vovinam 3",
          code: "VOV134",
          statusClass: "notpassed",
          status: "NotPassed",
          reason: "Sick",
        },
        {
          name: "Vovinam 1",
          code: "VOV114",
          statusClass: "passed",
          status: "Passed",
          reason: "",
        },
        {
          name: "Transition",
          code: "TRS6",
          statusClass: "passed",
          status: "Passed",
          reason: "",
        },
        {
          name: "Internet of Things",
          code: "IOT101",
          statusClass: "passed",
          status: "Passed",
          reason: "",
        },
        {
          name: "Mathematics for Engineering",
          code: "MAE101",
          statusClass: "passed",
          status: "Passed",
          reason: "",
        },
        {
          name: "Computer Organization and Architecture",
          code: "CEA201",
          statusClass: "passed",
          status: "Passed",
          reason: "",
        },
        {
          name: "Connecting to Computer Science",
          code: "CSI101",
          statusClass: "passed",
          status: "Passed",
          reason: "",
        },
        {
          name: "Programming Fundamentals",
          code: "PRF192",
          statusClass: "passed",
          status: "Passed",
          reason: "",
        },
        {
          name: "Working in Group Skills",
          code: "SSG101",
          statusClass: "passed",
          status: "Passed",
          reason: "",
        },
        {
          name: "Introduction to Databases",
          code: "DBI202",
          statusClass: "passed",
          status: "Passed",
          reason: "",
        },
        {
          name: "Object-Oriented Programming",
          code: "PRO192",
          statusClass: "passed",
          status: "Passed",
          reason: "",
        },
        {
          name: "Discrete mathematics",
          code: "MAD101",
          statusClass: "passed",
          status: "Passed",
          reason: "",
        },
        {
          name: "C Lab",
          code: "LAB101",
          statusClass: "passed",
          status: "Passed",
          reason: "",
        },
        {
          name: "Web Design",
          code: "WED201c",
          statusClass: "passed",
          status: "Passed",
          reason: "",
        },
        {
          name: "Desktop Java Applications",
          code: "PRJ311",
          statusClass: "passed",
          status: "Passed",
          reason: "",
        },
        {
          name: "OOP with Java Lab",
          code: "LAB211",
          statusClass: "passed",
          status: "Passed",
          reason: "",
        },
        {
          name: "Operating Systems",
          code: "OSG202",
          statusClass: "passed",
          status: "Passed",
          reason: "",
        },
        {
          name: "Data Structures and Algorithms",
          code: "CSD201",
          statusClass: "passed",
          status: "Passed",
          reason: "",
        },
        {
          name: "Elementary Japanese 1.1",
          code: "JPD111",
          statusClass: "passed",
          status: "Passed",
          reason: "",
        },
        {
          name: "Introduction to Software Engineering",
          code: "SWE102",
          statusClass: "study",
          status: "Studying",
          reason: "",
        },
        {
          name: "Desktop Java Lab",
          code: "LAB221",
          statusClass: "study",
          status: "Studying",
          reason: "",
        },
        {
          name: "Computer Networking",
          code: "NWC203c",
          statusClass: "study",
          status: "Studying",
          reason: "",
        },
        {
          name: "Japanese Elememtary 1-A1.2",
          code: "JPD123",
          statusClass: "study",
          status: "Studying",
          reason: "",
        },
        {
          name: "Web-Based Java Applications",
          code: "PRJ321",
          statusClass: "study",
          status: "Studying",
          reason: "",
        },
        {
          name: "Start Your Business",
          code: "SYB301",
          statusClass: "passed",
          status: "Passed",
          reason: "",
        },
      ],
    };
  },
};
</script>

<style scoped>
.notpassed {
  color: white;
  border-radius: 4px;
  padding: 0.2em 0.5em;
  background-color: red;
}
.passed {
  color: white;
  border-radius: 4px;
  padding: 0.2em 0.5em;
  background-color: green;
}
.study {
  color: white;
  border-radius: 4px;
  padding: 0.2em 0.5em;
  background-color: rgb(0, 183, 255);
}
</style>