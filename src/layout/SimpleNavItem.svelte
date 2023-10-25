<script>
    import { page } from '$app/stores';
    export let icon, title, url;

    $: active = $page.url.pathname === url ? 'active' : '';

</script>

<li class="menu {active}">
    <a href="{url}" aria-expanded="false" class="dropdown-toggle">
        <div class="align-middle">
            <i class="{icon}" style="font-size: 25px"></i>
            <span>{title}</span>
        </div>
    </a>
</li>

<style>

</style>