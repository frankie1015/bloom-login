<template>
    <div>
        <b-navbar
            toggleable="lg"
            type="light"
            variant="light"
            class="fixed-top"
        >
            <b-navbar-brand href="#">BLOOM</b-navbar-brand>

            <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

            <b-collapse id="nav-collapse" is-nav>
                <b-navbar-nav>
                    <b-nav-item href="#" class="border-left">Home</b-nav-item>
                    <b-nav-item href="#" class="border-left"
                        >Customer</b-nav-item
                    >
                    <b-nav-item href="#" class="border-left"
                        >Product</b-nav-item
                    >
                    <b-nav-item href="#" class="border-left"
                        >Placeholder</b-nav-item
                    >
                    <b-nav-item href="#" class="border-left"
                        >Placeholder</b-nav-item
                    >
                    <b-nav-item href="#" class="border-left"
                        >Placeholder</b-nav-item
                    >
                </b-navbar-nav>

                <!-- Right aligned nav items -->
                <b-navbar-nav class="ml-auto">
                    <b-nav-form>
                        <b-form-input
                            size="sm"
                            class="mr-sm-2"
                            placeholder="Search"
                        ></b-form-input>
                        <b-button size="sm" class="my-2 my-sm-0" type="submit"
                            >Search</b-button
                        >
                    </b-nav-form>

                    <b-nav-item-dropdown right>
                        <!-- Using 'button-content' slot -->
                        <template #button-content>
                            <em>User</em>
                        </template>
                        <b-dropdown-item href="#">Profile</b-dropdown-item>
                        <b-dropdown-item href="#">Sign Out</b-dropdown-item>
                    </b-nav-item-dropdown>
                </b-navbar-nav>
            </b-collapse>
        </b-navbar>
    </div>
</template>

<style>
.fixed-top {
    position: fixed;
    top: 0;
    left: 0;
    right: 0;
    z-index: 999;
}
</style>

<script>
export default {
    name: "navBar",
};
</script>
