<template>
  <div>
    <button @click="sendGet">get</button>
    <button @click="sendPost">post</button>
    <button @click="sendPut">put</button>
    <button @click="sendDelete">delete</button>
  </div>
</template>

<script>
import axios from 'axios'
export default {
  name: 'Axios',
  methods: {
    sendGet() {
      axios.get('https://enunau8irul5.x.pipedream.net')
    },
    sendPost() {
      axios.post('https://enunau8irul5.x.pipedream.net', {
        traQID: 'to-hutohu',
        grade: 16,
      })
    },
    sendPut() {
      axios.put('https://enunau8irul5.x.pipedream.net', {
        testData: { string: 'string', number: 1 },
      })
    },
    sendDelete() {
      axios.delete('https://enunau8irul5.x.pipedream.net', {
        data: { po: 1 },
      })
    },
  },
}
</script>
