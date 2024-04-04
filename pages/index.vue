<template>
    <div>
        <div class="layout">
            <header>
                <div class="header">
                    <div class="header-left">
                        <h1>How much?</h1>
                    </div>
                    
                    <div class="header-right">
                        <a-button>
                            <EditOutlined />
                        </a-button>
                    </div>
                </div>
            </header>
            <nav>
                <a-anchor
                    direction="horizontal"
                    :items="[
                        {
                            key: 'horizontally-part-1',
                            href: '#horizontally-part-1',
                            title: '통합',
                        },
                        {
                            key: 'horizontally-part-2',
                            href: '#horizontally-part-2',
                            title: '관리비',
                        },
                        {
                            key: 'horizontally-part-3',
                            href: '#horizontally-part-3',
                            title: '가스비',
                        },
                        {
                            key: 'horizontally-part-4',
                            href: '#horizontally-part-4',
                            title: '구독료',
                        }
                    ]"/>
            </nav>
         </div>
        </div>
</template>

<script setup lang="ts">


</script>

<style scoped>
.header {
    display: flex;
    justify-content: space-between;
}

.header-left {
    display: flex;
    position: left;
}

.header-right {
    margin-top: 40px;
    display: flex;
    position: right;
}
</style>