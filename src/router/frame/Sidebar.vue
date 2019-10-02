<template>
  <sidebar-menu :menu="menu" />
</template>
 
<script>
export default {
  data() {
    return {
      menu: [
        {
          header: true,
          title: 'Main Navigation',
          hiddenOnCollapse: true
        },
        {
          href: "/Dashboard",
          title: "Dashboard",
          icon: 'fas fa-tachometer-alt',
        },
        {
          href: "/Subjects",
          title: "Subjects",
          icon: 'fas fa-book',
        },
        {
          href: "/PersonalInfo",
          title: "Personal Info",
          icon: 'fas fa-user',
        },
        {
          href: "/Login",
          title: "Logout",
          icon: 'fas fa-sign-out-alt',
        }
      ]
    };
  }
};
</script> 