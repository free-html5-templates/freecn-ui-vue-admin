<template>
  <div class="flex h-[calc(90dvh)] flex-col items-center justify-center p-4 md:px-5 py-5 gap-4">
    <div class="border rounded-lg w-full h-full text-sm lg:flex">
      <ChatResizable :items="items"/>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import ChatResizable from '@/views/components/chat/resizable/ChatResizable.vue'
import { Chat } from '@/views/components/chat/Chat.ts'

export default defineComponent({
  name: 'ChatResizableHome',
  components: { ChatResizable },
  data()
  {
    return {
      items: [
        {
          id: 1,
          selected: true,
          user: {
            name: 'devlive',
            avatar: 'https://cdn.north.devlive.org/devlive.org/2024-04-17/2F28BD8A-5AB4-46BA-B614-287A0020FAE7.png'
          },
          messages: [
            {
              id: 1,
              content: 'Hello, how are you?',
              user: {
                name: 'devlive',
                avatar: 'https://cdn.north.devlive.org/devlive.org/2024-04-17/2F28BD8A-5AB4-46BA-B614-287A0020FAE7.png'
              },
              type: 'sender'
            },
            {
              id: 2,
              content: 'Hello, i am fine, and you?',
              user: {
                name: 'datacap',
                avatar: 'https://github.com/devlive-community/datacap/raw/dev/core/datacap-ui/public/static/images/logo.png'
              },
              type: 'receiver'
            },
            {
              id: 3,
              content: 'Hello, i love open source. How are you? I am fine, and you? What about you?',
              user: {
                name: 'devlive',
                avatar: 'https://cdn.north.devlive.org/devlive.org/2024-04-17/2F28BD8A-5AB4-46BA-B614-287A0020FAE7.png'
              },
              type: 'sender'
            },
            {
              id: 4,
              content: 'Hello, i love open source. How are you? I love freecn ui vue admin template and datacap and open ai java sdk. I am fine, and you? What about you?',
              user: {
                name: 'datacap',
                avatar: 'https://github.com/devlive-community/datacap/raw/dev/core/datacap-ui/public/static/images/logo.png'
              },
              type: 'receiver'
            },
            {
              id: 5,
              content: 'Hello, i love open source. How are you? I love freecn ui vue admin template and datacap and open ai java sdk. I am fine, and you? What about you?',
              user: {
                name: 'devlive',
                avatar: 'https://cdn.north.devlive.org/devlive.org/2024-04-17/2F28BD8A-5AB4-46BA-B614-287A0020FAE7.png'
              },
              type: 'sender'
            },
            {
              id: 6,
              content: 'Hello, i love open source. How are you? I love freecn ui vue admin template and datacap and open ai java sdk. I am fine, and you? What about you?',
              user: {
                name: 'datacap',
                avatar: 'https://github.com/devlive-community/datacap/raw/dev/core/datacap-ui/public/static/images/logo.png'
              },
              type: 'receiver'
            },
            {
              id: 7,
              content: 'Hello, i love open source. How are you? I love freecn ui vue admin template and datacap and open ai java sdk. I am fine, and you? What about you?',
              user: {
                name: 'devlive',
                avatar: 'https://cdn.north.devlive.org/devlive.org/2024-04-17/2F28BD8A-5AB4-46BA-B614-287A0020FAE7.png'
              },
              type: 'sender'
            },
            {
              id: 8,
              content: 'Hello, i love open source. How are you? I love freecn ui vue admin template and datacap and open ai java sdk. I am fine, and you? What about you?',
              user: {
                name: 'datacap',
                avatar: 'https://github.com/devlive-community/datacap/raw/dev/core/datacap-ui/public/static/images/logo.png'
              },
              type: 'receiver'
            }
          ]
        },
        {
          id: 2,
          user: {
            name: 'datacap',
            avatar: 'https://github.com/devlive-community/datacap/raw/dev/core/datacap-ui/public/static/images/logo.png'
          },
          messages: [
            {
              id: 11,
              content: 'Hello, i am fine, and you?',
              user: {
                name: 'datacap',
                avatar: 'https://github.com/devlive-community/datacap/raw/dev/core/datacap-ui/public/static/images/logo.png'
              },
              type: 'sender'
            }
          ]
        },
        {
          id: 3,
          user: {
            name: 'qianmoQ',
            avatar: 'https://avatars.githubusercontent.com/u/20521442?s=64&v=4'
          },
          messages: [
            {
              id: 21,
              content: 'Hello, i love open source. How are you? I am fine, and you? What about you?',
              user: {
                name: 'qianmoQ',
                avatar: 'https://avatars.githubusercontent.com/u/20521442?s=64&v=4'
              }
            }
          ]
        }
      ] as Chat[]
    }
  }
})
</script>
