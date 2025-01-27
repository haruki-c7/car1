<template>
 <PageLayout
  type="three-columns"
  theme="dark"
  class="luxury-theme"
 >
  <template #header>
   <ShareHeaderDocs
    class="luxury-header"
   />
  </template>
  <template #start>
   <ViewState
    v-slot="navigation"
    src="route://meta"
    path="navigation"
   >
    <Sidebar
     id="sidebar"
     active-background-color="#b08d57"
     background-color="#1e1e2d"
     text-color="#ffffff"
     border-radius="8px"
     shadow="xl"
     :src="`app-config://usebootstrap/navigations/${navigation.data || 'default'}`"
    />
   </ViewState>
  </template>
  <template #end>
   <Toc
    selector="#content"
    display="none lg-block print-none"
    color="#b08d57"
    font-size="16px"
   >
    <Localization>
     <template #en>
      On this page
     </template>
     <template #ja>
      項目
     </template>
    </Localization>
   </Toc>
  </template>
  <template #default>
   <b-div
    id="content"
    class="luxury-content"
    padding="4xl"
    border-radius="xl"
    background-color="#2b2b3d"
   >
    <slot />
   </b-div>
  </template>
  <template #footer>
   <ShareFooter
    class="luxury-footer"
    background-color="#1e1e2d"
    text-color="#b08d57"
   />
  </template>
 </PageLayout>
</template>

<style scoped>
.luxury-theme {
  font-family: "Merriweather", serif;
  color: #f4f4f7;
  background-color: #1e1e2d;
}
.luxury-header {
  background: linear-gradient(90deg, #1e1e2d, #3a3a4d);
  padding: 20px;
  border-bottom: 2px solid #b08d57;
}
.luxury-content {
  box-shadow: 0px 10px 30px rgba(0, 0, 0, 0.5);
}
.luxury-footer {
  text-align: center;
  padding: 20px;
  border-top: 2px solid #b08d57;
}
</style>
