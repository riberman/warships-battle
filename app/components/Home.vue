<template>
    <Page class="page">
      <ActionBar title="Master" />
        <StackLayout>
          <Button text="To Details directly" @tap="goToLogin" />
        </StackLayout>
    </Page>
</template>

<script>
import Login from './Login';

export default {
data () {
    return {
    };
},
methods: {
    goToLogin() {
        this.$navigateTo(Login)
    }
}
}
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
