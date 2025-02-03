<template>
  <PageLayout type="three-columns" theme="dark" class="text-white bg-black">
    <template #header>
      <ShareHeaderDocs class="bg-dark border-bottom border-warning p-3" />
    </template>
    <template #start>
      <ViewState v-slot="navigation" src="route://meta" path="navigation">
        <Sidebar
          id="sidebar"
          class="bg-dark text-white shadow-lg rounded"
          :src="`app-config://usebootstrap/navigations/${navigation.data || 'default'}`"
        />
      </ViewState>
    </template>
    <template #end>
      <Toc selector="#content" class="d-none d-lg-block d-print-none text-warning fs-5">
        <Localization>
          <template #en> On this page </template>
        </Localization>
      </Toc>
    </template>
    <template #default>
      <div id="content" class="p-5 rounded bg-dark shadow-lg">
        <slot />
      </div>
    </template>
    <template #footer>
      <ShareFooter class="bg-dark text-warning text-center p-3 border-top border-warning" />
    </template>
  </PageLayout>
</template>
