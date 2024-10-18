<script>
  export default {
    data () {
      return {
        team: [
          {
            name: 'Anna Becker',
            role: 'Developer',
          },
          {
            name: 'Anne Quinkenstein',
            role: 'Developer',
          },
          {
            name: 'Charlene Zander',
            role: 'Product Owner, Developer',
          },
          {
            name: 'Michael Haughey',
            role: 'Battery Systems Engineer',
          },
          {
            name: 'Leona Schulz',
            role: 'Developer',
          },
          {
            name: 'Jennifer Luu',
            role: 'Scrum Master',
          },
          {
            name: 'Theertha Sunesh',
            role: 'Developer',
          }
        ],
      }
    },
  }
</script>
<template>
    <v-row class="mt-5">
        <v-col cols="3">
            <img src="../assets/our-team.jpg" alt="Projekt" style="width: 100%">
        </v-col>
        <v-col cols="9">
            <p class="text-h4 font-weight-bold mb-3 heading-color">Team</p>
            <v-table>
                <thead>
                    <tr>
                        <th class="text-left font-weight-bold text-h6">
                        Name
                        </th>
                        <th class="text-left font-weight-bold text-h6">
                        Role
                        </th>
                    </tr>
                </thead>
                <tbody>
                    <tr
                        v-for="item in team"
                        :key="item.name"
                    >
                        <td>{{ item.name }}</td>
                        <td>{{ item.role }}</td>
                    </tr>
                </tbody>
            </v-table>
        </v-col>
    </v-row>
</template>