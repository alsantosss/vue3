<template>
    <div>
        <img :src="avatar" :title="avatar_desc" width="100" height="120">
    </div>
</template>

<script>
export default {
    nome:"avatar",
    data(){
        return {
            avatar: "/img/avatar.svg",
            avatar_desc:"avatar"
        }
    }
}
</script>