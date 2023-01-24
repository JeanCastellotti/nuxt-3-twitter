<script setup></script>

<template>
  <div class="hidden xs:col-span-1 md:block xl:col-span-2">
    <div class="sticky top-0">
      <TheLogo />

      <SidebarLeftTab active>
        <template #icon>
          <Icon name="heroicons:home-solid" size="24px" />
        </template>
        <template #label>Home</template>
      </SidebarLeftTab>

      <SidebarLeftTab>
        <template #icon>
          <Icon name="heroicons:hashtag-solid" size="24px" />
        </template>
        <template #label>Explore</template>
      </SidebarLeftTab>

      <SidebarLeftTab>
        <template #icon>
          <Icon name="heroicons:bell-solid" size="24px" />
        </template>
        <template #label>Notifications</template>
      </SidebarLeftTab>

      <SidebarLeftTab>
        <template #icon>
          <Icon name="heroicons:inbox-solid" size="24px" />
        </template>
        <template #label>Messages</template>
      </SidebarLeftTab>

      <SidebarLeftTab>
        <template #icon>
          <Icon name="heroicons:bookmark-solid" size="24px" />
        </template>
        <template #label>Bookmarks</template>
      </SidebarLeftTab>

      <SidebarLeftTab>
        <template #icon>
          <Icon name="heroicons:document-text-solid" size="24px" />
        </template>
        <template #label>Lists</template>
      </SidebarLeftTab>

      <SidebarLeftTab>
        <template #icon>
          <Icon name="heroicons:user-circle-solid" size="24px" />
        </template>
        <template #label>Profile</template>
      </SidebarLeftTab>

      <SidebarLeftTab>
        <template #icon>
          <Icon name="heroicons:ellipsis-horizontal-circle-solid" size="24px" />
        </template>
        <template #label>More</template>
      </SidebarLeftTab>
    </div>
  </div>
</template>
