<template>
    <div>
        <div class="min-h-screen bg-gray-100">
<!--            <nav class="bg-white border-b border-gray-100">-->
<!--                &lt;!&ndash; Primary Navigation Menu &ndash;&gt;-->
<!--                <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">-->
<!--                    <div class="flex justify-between h-16">-->
<!--                        <div class="flex">-->
<!--                            &lt;!&ndash; Logo &ndash;&gt;-->
<!--                            <div class="flex-shrink-0 flex items-center">-->
<!--                                <Link :href="route('dashboard')">-->
<!--                                    <BreezeApplicationLogo class="block h-9 w-auto" />-->
<!--                                </Link>-->
<!--                            </div>-->

<!--                            &lt;!&ndash; Navigation Links &ndash;&gt;-->
<!--                            <div class="hidden space-x-8 sm:-my-px sm:ml-10 sm:flex">-->
<!--                                <BreezeNavLink>-->
<!--                                    Link 1-->
<!--                                </BreezeNavLink>-->
<!--                                <BreezeNavLink>-->
<!--                                    Link 2-->
<!--                                </BreezeNavLink>-->
<!--                                <BreezeNavLink>-->
<!--                                    Link 3-->
<!--                                </BreezeNavLink>-->
<!--&lt;!&ndash;                                <BreezeNavLink :href="route('welcome')" :active="route().current('welcome')">&ndash;&gt;-->
<!--&lt;!&ndash;                                    Wekcome&ndash;&gt;-->
<!--&lt;!&ndash;                                </BreezeNavLink>&ndash;&gt;-->
<!--                            </div>-->
<!--                        </div>-->
<!--                        <div class="hidden sm:flex sm:items-center sm:ml-6">-->
<!--                            &lt;!&ndash; Settings Dropdown &ndash;&gt;-->
<!--                            <div class="ml-3 relative">-->
<!--                                <BreezeDropdown align="right" width="48">-->
<!--                                    <template #trigger>-->
<!--                                        <span class="inline-flex rounded-md">-->
<!--&lt;!&ndash;                                            <button type="button" class="inline-flex items-center px-3 py-2 border border-transparent text-sm leading-4 font-medium rounded-md text-gray-500 bg-white hover:text-gray-700 focus:outline-none transition ease-in-out duration-150">&ndash;&gt;-->
<!--&lt;!&ndash;                                                {{ $page.props.auth.user.name }}&ndash;&gt;-->

<!--&lt;!&ndash;                                                <svg class="ml-2 -mr-0.5 h-4 w-4" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20" fill="currentColor">&ndash;&gt;-->
<!--&lt;!&ndash;                                                    <path fill-rule="evenodd" d="M5.293 7.293a1 1 0 011.414 0L10 10.586l3.293-3.293a1 1 0 111.414 1.414l-4 4a1 1 0 01-1.414 0l-4-4a1 1 0 010-1.414z" clip-rule="evenodd" />&ndash;&gt;-->
<!--&lt;!&ndash;                                                </svg>&ndash;&gt;-->
<!--&lt;!&ndash;                                            </button>&ndash;&gt;-->
<!--                                        </span>-->
<!--                                    </template>-->

<!--                                    <template #content>-->
<!--                                        <BreezeDropdownLink method="post" as="button">-->
<!--                                            Test-->
<!--                                        </BreezeDropdownLink>-->
<!--                                    </template>-->
<!--                                </BreezeDropdown>-->
<!--                            </div>-->
<!--                        </div>-->

<!--                        &lt;!&ndash; Hamburger &ndash;&gt;-->
<!--                        <div class="-mr-2 flex items-center sm:hidden">-->
<!--                            <button @click="showingNavigationDropdown = ! showingNavigationDropdown" class="inline-flex items-center justify-center p-2 rounded-md text-gray-400 hover:text-gray-500 hover:bg-gray-100 focus:outline-none focus:bg-gray-100 focus:text-gray-500 transition duration-150 ease-in-out">-->
<!--                                <svg class="h-6 w-6" stroke="currentColor" fill="none" viewBox="0 0 24 24">-->
<!--                                    <path :class="{'hidden': showingNavigationDropdown, 'inline-flex': ! showingNavigationDropdown }" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16" />-->
<!--                                    <path :class="{'hidden': ! showingNavigationDropdown, 'inline-flex': showingNavigationDropdown }" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12" />-->
<!--                                </svg>-->
<!--                            </button>-->
<!--                        </div>-->
<!--                    </div>-->
<!--                </div>-->

<!--                &lt;!&ndash; Responsive Navigation Menu &ndash;&gt;-->
<!--                <div :class="{'block': showingNavigationDropdown, 'hidden': ! showingNavigationDropdown}" class="sm:hidden">-->
<!--                    <div class="pt-2 pb-3 space-y-1">-->
<!--                        <BreezeResponsiveNavLink :href="route('dashboard')" :active="route().current('dashboard')">-->
<!--                            Dashboard-->
<!--                        </BreezeResponsiveNavLink>-->
<!--                    </div>-->

<!--                    &lt;!&ndash; Responsive Settings Options &ndash;&gt;-->
<!--                    <div class="pt-4 pb-1 border-t border-gray-200">-->
<!--                        <div class="px-4">-->
<!--&lt;!&ndash;                            <div class="font-medium text-base text-gray-800">{{ $page.props.auth.user.name }}</div>&ndash;&gt;-->
<!--&lt;!&ndash;                            <div class="font-medium text-sm text-gray-500">{{ $page.props.auth.user.email }}</div>&ndash;&gt;-->
<!--                        </div>-->

<!--                        <div class="mt-3 space-y-1">-->
<!--                            <BreezeResponsiveNavLink :href="route('logout')" method="post" as="button">-->
<!--                                Log Out-->
<!--                            </BreezeResponsiveNavLink>-->
<!--                        </div>-->
<!--                    </div>-->
<!--                </div>-->
<!--            </nav>-->

            <!-- Page Heading -->
        <Header></Header>
            <!-- Page Content -->
            <main>
                <slot />
            </main>
            <!-- Page Footer -->
            <Footer>
            </Footer>
        </div>
    </div>
</template>

<script>
import BreezeApplicationLogo from '@/Components/ApplicationLogo.vue'
import BreezeDropdown from '@/Components/Dropdown.vue'
import BreezeDropdownLink from '@/Components/DropdownLink.vue'
import BreezeNavLink from '@/Components/NavLink.vue'
import BreezeResponsiveNavLink from '@/Components/ResponsiveNavLink.vue'
import { Link } from '@inertiajs/inertia-vue3';
import Header from "@/Components/LandingPage/Header";
import Footer from "@/Components/LandingPage/Footer";

export default {
    components: {
        Footer,
        Header,
        BreezeApplicationLogo,
        BreezeDropdown,
        BreezeDropdownLink,
        BreezeNavLink,
        BreezeResponsiveNavLink,
        Link,
    },

    data() {
        return {
            showingNavigationDropdown: false,
        }
    },
}
</script>

<style scoped>

</style>
