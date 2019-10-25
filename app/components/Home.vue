<template>
    <Page class="page">
      <ActionBar title="SideDrawer Button">
          <android>
            <NavigationButton icon="res://ic_menu" tap="showSideDrawer" />
          </android>
          <ios>
            <ActionItem icon="res://ic_menu" tap="showSideDrawer" />
          </ios>
        </ActionBar>
    </Page>
</template>

<script>
    export default {
        computed: {
            message() {
                return "Blank {N}-Vue app";
            }
        }
    };
</script>

<style scoped lang="scss">
    // Start custom common variables
    @import '../app-variables';
    // End custom common variables

    // Custom styles
    .fa {
        color: $accent-dark;
    }

    .info {
        font-size: 20;
    }

    .action-bar {
        text-align: left;
        background-color: #34495e;
    }
</style>
