<template>
  <AppColorMode>
    <AppWrapper>
      <AppGrid>
        <SidebarLeft />
        <main class="col-span-12 md:col-span-8 xl:col-span-6">
          <NuxtPage />
        </main>
        <SidebarRight />
      </AppGrid>
    </AppWrapper>
  </AppColorMode>
</template>
