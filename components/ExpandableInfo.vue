<template>
  <v-row no-gutters>
    <v-col>
      <h1>
        {{ title }}
      </h1>
      <p>
        {{ desc }}
      </p>
    </v-col>
    <v-col cols="3">
      <!-- Significantly less dry w/ Vue iterator directive! -->
      <v-expansion-panels multiple>
        <v-expansion-panel v-for="t in topics" :key="t.title">
          <v-expansion-panel-title>{{ t.title }}</v-expansion-panel-title>
          <v-expansion-panel-text>
            <v-expansion-panels>
              <v-expansion-panel v-for="s in t.subtopics" :key="s.title">
                <v-expansion-panel-title @click="change(s.title, s.desc)">
                  {{ s.title }}
                </v-expansion-panel-title>
                <v-expansion-panel-text @click="change(s.title, s.desc)">
                  {{ s.desc }}
                </v-expansion-panel-text>
              </v-expansion-panel>
            </v-expansion-panels>
          </v-expansion-panel-text>
        </v-expansion-panel>
      </v-expansion-panels>
    </v-col>
  </v-row>
</template>

<script>
export default {
  name: 'ExpandableInfo',
  data () {
    return {
      title: 'Title Here',
      desc: 'When you select a topic from the right, the title above will chance dynamically and this description you are reading here will change as well.',
      topics: [ // Move data into a json file to import instead for more modularity?
        {
          title: 'Data Structures',
          subtopics: [
            { title: 'Stack', desc: 'LIFO' },
            { title: 'Queue', desc: 'FIFO' },
            { title: 'Linked List', desc: 'TBA' },
            { title: 'Heap', desc: 'TBA' },
            { title: 'Hash Table', desc: 'TBA' },
            { title: 'Tree', desc: 'TBA: Binary Search Trees, Red-Black Trees, B-Trees, Graphs, etc.' },
            { title: 'Graph', desc: 'TBA: Directed Acyclical Graphs, etc.' }
          ]
        },
        {
          title: 'Algorithms',
          subtopics: [
            { title: 'Sorting Algorithms', desc: 'TBA: Heapsort, Quicksort, Bubblesort' },
            { title: 'Graph Algorithms', desc: 'TBA: Breadth-first search, Depth-first search, topological sort, etc' },
            { title: 'Greedy Algorithms', desc: 'TBA' }
          ]
        },
        {
          title: 'Design Patterns',
          subtopics: [
            { title: 'Singleton', desc: 'TBA' },
            { title: 'Factory', desc: 'TBA' },
            { title: 'Builder', desc: 'TBA' }
          ]
        },
        {
          title: 'Prog Lang Syntax',
          subtopics: [
            { title: 'Java', desc: 'TBA' },
            { title: 'C#', desc: 'TBA' },
            { title: 'Python', desc: 'TBA' }
          ]
        }
      ]
    }
  },
  methods: {
    change (title, desc) {
      this.title = title
      this.desc = desc
    }
  }
}
</script>
