
<template>
    <div class="flex-center position-ref full-height">
        <div class="content">
            <div class="title m-b-md">
                {{title}}
            </div>

            <div class="links">
                <span class="subtitle">Name : {{author.name}}</span><br/>
                <span class="subtitle">Role : {{author.role}}</span><br/>
                <span class="subtitle">Code : {{author.code}}</span><br/>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        props : ['title', 'author']
    }
</script>
<style scoped>
    html, body {
        background-color: #fff;
        color: #939b9f;
        font-family: 'Raleway', sans-serif;
        font-weight: 100;
        height: 100vh;
        margin: 0;
    }
    .title {
        font-size: 60px;
    }
    .subtitle {
        font-size: 20px;
    }
    .full-height {
        height: 100vh;
    }

    .flex-center {
        align-items: center;
        display: flex;
        justify-content: center;
    }
    .position-ref {
        position: relative;
    }

    .top-right {
        position: absolute;
        right: 10px;
        top: 18px;
    }
    .content {
        text-align: center;
    }
    .m-b-md {
        margin-bottom: 30px;
    }
</style>