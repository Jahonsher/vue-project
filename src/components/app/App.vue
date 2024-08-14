<template>
<div class="app">
    <div class="content">
        <Appinfo />
        <div class="search-panel">
            <SearchPanel />
            <AppFilter />
        </div>
        <MoviList />
        <MoviAddForm />
    </div>
</div>
</template>


<script>
import Appinfo from '@/components/app-info/Appinfo.vue';
import SearchPanel from '../seach-panel/SearchPanel.vue';
import AppFilter from '../App-filter/AppFilter.vue';
import MoviList from '../Movi-list/MoviList.vue';
import MoviAddForm from '../Movi-Add-Form/MoviAddForm.vue';

    export default {
        components: {
            Appinfo,
            SearchPanel,
            AppFilter,
            MoviList,
            MoviAddForm
        }
    }
</script>

<style>
.app {
    height: 100vh;
    color: #000
}

.content {
    width: 1000px;
    min-height: 700px;
    background-color: #fff;
    margin: 0 auto;
    padding: 5rem 10px;
}

.search-panel {
    margin-top: 2rem;
    padding: 1.5rem;
    background-color: #fcfaf5;
    border-radius: 4px;
    box-shadow: 15px 15px 15px rgb(0, 0, 0 , 0.15);
}

</style>