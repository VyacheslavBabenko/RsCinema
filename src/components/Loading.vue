<template>
    <div class="ball-wrapper">
        <div class="ball"></div>
    </div>
</template>

<script>
export default {
    name: 'loading',
}
</script>

<style lang="scss" scoped>

.ball-wrapper {
    position: relative;
    display: flex;
    justify-content: center;
    height: 100vh;
    align-items: center;
}
.ball {
    border: 5px solid ;
    border-color: #FAB200;
    opacity: .9;
    border-top: 5px solid rgba(0,0,0,0);
    border-left: 5px solid rgba(0,0,0,0);
    border-radius: 50px;
    width: 50px;
    height: 50px;
    margin: 0 auto;
    -moz-animation: spin .9s infinite linear;
    -webkit-animation: spin .9s infinite linear;
}

@-moz-keyframes spin {
    0% { -moz-transform:rotate(0deg); }
    100% { -moz-transform:rotate(360deg); }
}
@-moz-keyframes spinoff {
    0% { -moz-transform:rotate(0deg); }
    100% { -moz-transform:rotate(-360deg); }
}
@-webkit-keyframes spin {
    0% { -webkit-transform:rotate(0deg); }
    100% { -webkit-transform:rotate(360deg); }
}
@-webkit-keyframes spinoff {
    0% { -webkit-transform:rotate(0deg); }
    100% { -webkit-transform:rotate(-360deg); }
}
</style>