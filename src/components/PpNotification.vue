<template>
  <div class="pp-notifications pp-display-none" id="notifications_dropdown">
    <header>
        <h2>Notifications
            <a href="#" class="pp-ico-close"></a>
        </h2>
    </header>
    <section>
        <ul class="pp-no-margin-top">
            <li class="pp-fake-loader" style="">
                <span class="pp-fake-content">
                                        <span></span>
                <span class="small"></span>
                </span>
            </li>
        </ul>
    </section>
    <footer>
        <a class="pp-btn" href="/notifications">View all notifications</a>
    </footer>
</div>
</template>

<script>
    module.exports = {
      name: 'ppNotification'
    }
</script>
