<template>
    <div class="pp-dropdown" id="menu" style="top: 52.5px; left: 861px;">
        <div class="pp-dropdown-body">
            <ul class="pp-dropdown-content">
                <li>
                    <a class="pp-ico-my-desk" href="/my_desk">MyDesk</a>
                </li>
                <li>
                    <a class="pp-ico-home" href="/organizations/switch">Switch Organization</a>
                </li>
                <li>
                    <a class="pp-ico-cog" href="/users/71859/edit">User Settings</a>
                </li>
                <li>
                    <a class="pp-ico-cog" href="/organizations/53756/edit">Organization settings</a>
                </li>
                <li><a class="pp-ico-logout" rel="nofollow" data-method="delete" href="/logout">Logout</a></li>
            </ul>
        </div>
    </div>
</template>

<script>
    module.exports = {
      name: 'ppDropdown'
    }
</script>
