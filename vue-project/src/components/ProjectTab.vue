<script>
  export default {
    data () {
      return {
        team: [
          {
            name: 'Frontend UI',
            role: 'Vue 5, Figma',
          },
          {
            name: 'Backend',
            role: 'Spring Boot 5',
          },
          {
            name: 'Database Management',
            role: 'MongoDB 5',
          },
          {
            name: 'Logo Design',
            role: 'Midjourney AI V5, Lunapic',
          },
          {
            name: 'Task Management',
            role: 'Jira',
          },
          {
            name: 'Communication',
            role: 'Slack, Zoom',
          },
          {
            name: 'Version Control',
            role: 'Github',
          },
          {
            name: 'Project Documentation',
            role: 'Overleaf, Confluence',
          }
        ],
      }
    },
  }
</script>

<template>
    <v-row class="mt-5">
        <v-col cols="3">
            <img src="../assets/logo_logo.png" alt="Projekt" style="width: 100%">
        </v-col>
        <v-col cols="9">
            <p class="text-h4 font-weight-bold mb-3 heading-color">Project</p>
            <p class="text-h6 font-weight-medium mb-2 heading-color">The Goal and Task:</p>
            <p>The team was tasked with developing a battery passport to meet the newly proposed regulations.</p>
            <p>The primary goals of the passport including:</p>
            <p>1. Enabling transparency regarding the CO2 footprint of batteries</p>
            <p>2. Improve battery recycling</p>
            <p>3. Minimise human exploitation that commonly occurs during mining and extraction of the raw materials required for batteries.</p>
            
            <p class="text-h6 mt-3 mb-2 font-weight-medium heading-color">Involved Company:</p>
            <p>The company involved with the project is InMediasP. InMediasP deals with processes, products and product development with a focus on digital twins, end to end solutions and PLM.</p>
            
            <p class="text-h6 mt-3 mb-2 font-weight-medium heading-color"> Who Will Use it: </p>
            <p> 1.	Battery manufacturers (including cell, module, and battery manufacturers)</p>
            <p> 2.	EV vehicle manufacturers</p>
            <p> 3.	EV maintenance providers</p>
            <p> 4.	Battery recyclers</p>
            <p> 5.	Raw material producers</p>
            <p> 6.	Material processors</p>
            <p class="text-h6 mt-3 mb-2 font-weight-medium heading-color">Software Used:</p>


            <v-table>
                <thead>
                    <tr>
                        <th class="text-left font-weight-bold text-h6">
                        Function
                        </th>
                        <th class="text-left font-weight-bold text-h6">
                        Software Package
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