<script>
    import SimpleNavItem from "./SimpleNavItem.svelte";
</script>

<div class="sidebar-wrapper sidebar-theme">
    <nav id="sidebar">
        <div class="navbar-nav theme-brand flex-row  text-center">
            <div class="nav-logo">
                <div class="nav-item theme-logo">
                    <a href="/">
                        <img src="../images/logo.svg" class="navbar-logo" alt="logo">
                    </a>
                </div>
                <div class="nav-item theme-text">
                    <a href="/" class="nav-link"> CORK </a>
                </div>
            </div>
            <div class="nav-item sidebar-toggle">
                <div class="btn-toggle sidebarCollapse">
                    <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none"
                         stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"
                         class="feather feather-chevrons-left">
                        <polyline points="11 17 6 12 11 7"></polyline>
                        <polyline points="18 17 13 12 18 7"></polyline>
                    </svg>
                </div>
            </div>
        </div>

        <ul class="list-unstyled menu-categories" id="accordionExample">
            <!--<li class="menu active">
                <a href="/" aria-expanded="true" class="dropdown-toggle">
                    <div class="">
                        <i class="ti ti-home ti-2x"></i>
                        <span>Home</span>
                    </div>
                </a>
            </li>-->
            <SimpleNavItem icon="ti ti-home" title="Home" url="/" />
            <SimpleNavItem icon="ti ti-users" title="Home" url="/employees" />
            <SimpleNavItem icon="ti ti-users" title="Home" url="/employees" />
            <SimpleNavItem icon="ti ti-users" title="Home" url="/employees" />
            <li class="menu">
                <a href="blank-page.html" aria-expanded="false" class="dropdown-toggle">
                    <div class="">
                        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none"
                             stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"
                             class="feather feather-star">
                            <polygon
                                    points="12 2 15.09 8.26 22 9.27 17 14.14 18.18 21.02 12 17.77 5.82 21.02 7 14.14 2 9.27 8.91 8.26 12 2"></polygon>
                        </svg>
                        <span>Blank Page</span>
                    </div>
                </a>
            </li>

            <li class="menu menu-heading">
                <div class="heading">
                    <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none"
                         stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"
                         class="feather feather-minus">
                        <line x1="5" y1="12" x2="19" y2="12"></line>
                    </svg>
                    <span>MENU LEVELS</span></div>
            </li>

            <li class="menu">
                <a href="#home" data-bs-toggle="collapse" aria-expanded="false" class="dropdown-toggle">
                    <div class="">
                        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none"
                             stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"
                             class="feather feather-hash">
                            <line x1="4" y1="9" x2="20" y2="9"></line>
                            <line x1="4" y1="15" x2="20" y2="15"></line>
                            <line x1="10" y1="3" x2="8" y2="21"></line>
                            <line x1="16" y1="3" x2="14" y2="21"></line>
                        </svg>
                        <span>Level 1</span>
                    </div>
                    <div>
                        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none"
                             stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"
                             class="feather feather-chevron-right">
                            <polyline points="9 18 15 12 9 6"></polyline>
                        </svg>
                    </div>
                </a>
                <ul class="collapse submenu list-unstyled" id="home" data-bs-parent="#accordionExample">
                    <li>
                        <a href="javascript:void(0);"> Level 2a </a>
                    </li>
                    <li>
                        <a href="javascript:void(0);"> Level 2b </a>
                    </li>

                    <li>
                        <a href="#level-three" data-bs-toggle="collapse" aria-expanded="false"
                           class="dropdown-toggle collapsed"> Level 2c
                            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24"
                                 fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round"
                                 stroke-linejoin="round" class="feather feather-chevron-right">
                                <polyline points="9 18 15 12 9 6"></polyline>
                            </svg>
                        </a>
                        <ul class="collapse list-unstyled sub-submenu" id="level-three" data-bs-parent="#pages">
                            <li>
                                <a href="javascript:void(0);"> Level 3a </a>
                            </li>
                            <li>
                                <a href="javascript:void(0);"> Level 3b </a>
                            </li>
                            <li>
                                <a href="javascript:void(0);"> Level 3c </a>
                            </li>
                        </ul>
                    </li>
                </ul>
            </li>

        </ul>

    </nav>

</div>

<style>

</style>