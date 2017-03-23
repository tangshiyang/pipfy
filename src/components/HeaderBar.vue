<template>
    <header class="pp-header">
        <div class="pp-top-header">
            <div class="pp-left-side">
                <a href="/" class="pp-logo"></a>
                <a class="pp-org-name pp-no-after" href="/organizations/53756">{{orgName}}</a>
                <span class="pp-trial ">
                <a class="pp-btn-sm" href="#">功能升级</a>
            </span>
            </div>
            <div class="pp-right-side">
                <div id="notifications_popup" class="">
                    <a class="pull-left pp-header-actions glyphicon glyphicon-bell pp-xiaoxi-btn" id="notifications_button" href="#"></a>
                    <pp-notification></pp-notification>
                </div>
                <a href="#" class="pp-user-photo" data-pp-module="dropdown" data-target="#menu">
                    <img class="pp-avatar pp-round" v-bind:src="ppround"  alt="User avatar default">
                </a>
            </div>
        </div>
        <pp-dropdown></pp-dropdown>
    </header>
</template>

<script>
var ppNotification = require('./PpNotification')
var ppDropdown = require('./PpDropdown')
module.exports = {
  name: 'headerbar',
  data: function () {
    return {
      orgName: 'Wex',
      ppround: 'https://gravatar.com/avatar/c4b08c0b8ef7ef81a657393670018308.png?s=128&amp;d=https://app.pipefy.com/images/user-avatar-default.png'
    }
  },
  components: {
    'pp-notification': ppNotification,
    'pp-dropdown': ppDropdown
  }
}
</script>


<style scoped>
  .pp-trial {
    text-align: left;
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
  }
  .pp-xiaoxi-btn{
      margin-right: 15px;
      margin-left: 0;
      font-size: 26px;
      color: rgba(255,255,255,0.8);
      font-weight: normal;
  }
  .pp-header .pp-left-side .pp-trial a {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
  }
.pp-header .pp-right-side .pp-user-photo:after {
    position: absolute;
    font-family: "pipeicons";
    content: ".";
    font-size: 14px;
    color: rgba(255,255,255,0.8);
    top: 0;
    right: -15px;
    padding: 10px 0 10px 12px;
}
</style>
