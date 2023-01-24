<script setup>
const whatsHappeningItems = ref([
  {
    title: '#spacex',
    count: '18.8k',
  },
  {
    title: '#codingisfun',
    count: '15.6k',
  },
  {
    title: '#javascript',
    count: '12.1k',
  },
])

const whoToFollowItems = ref([
  {
    name: 'Joe Biden',
    handle: '@JoeBiden',
    image: 'https://picsum.photos/200/200',
  },
  {
    name: 'Joe Biden',
    handle: '@JoeBiden',
    image: 'https://picsum.photos/200/200',
  },
  {
    name: 'Joe Biden',
    handle: '@JoeBiden',
    image: 'https://picsum.photos/200/200',
  },
])
</script>

<template>
  <div class="hidden h-screen md:col-span-3 md:block xl:col-span-4">
    <div class="sticky top-0">
      <SidebarRightCard title="What's happening">
        <SidebarRightItem v-for="item in whatsHappeningItems">
          <h2 class="font-semibold text-slate-800 dark:text-slate-100">
            {{ item.title }}
          </h2>
          <span class="text-xs text-slate-500 dark:text-slate-400">
            {{ item.count }}
          </span>
        </SidebarRightItem>
      </SidebarRightCard>
      <SidebarRightCard title="Who to follow">
        <SidebarRightItem v-for="item in whoToFollowItems">
          <div class="flex items-center justify-between p-2">
            <div class="flex gap-2">
              <img
                :src="item.image"
                :alt="item.name"
                class="h-10 w-10 rounded-full"
              />
              <div>
                <h2
                  class="text-sm font-semibold text-slate-800 dark:text-slate-100"
                >
                  {{ item.name }}
                </h2>
                <span class="text-xs text-slate-400">{{ item.handle }}</span>
              </div>
            </div>
            <button
              class="rounded-full bg-slate-800 px-4 py-1.5 text-sm font-bold text-slate-100 dark:bg-slate-400 dark:text-slate-800"
            >
              Follow
            </button>
          </div>
        </SidebarRightItem>
      </SidebarRightCard>
    </div>
  </div>
</template>
