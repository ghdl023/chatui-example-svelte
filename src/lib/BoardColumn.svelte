<script>
    import BoardColumnItem from "./BoardColumnItem.svelte";

    export let columnName = '';
    export let items = [
        {'title': '제목'},
        {'title': '제목'},
        {'title': '제목'},
        {'title': '제목'},
    ];
</script>

<div class="board-column">
   <div class="board-colum-header">
       <h4>{columnName}</h4>
       <div class="btn-plus">
           <button>+</button>
       </div>
   </div>

    {#each items as item}
        <BoardColumnItem item={item} />
    {/each}
    <div>
        <button>+ Add task</button>
    </div>
</div>

<style>
    .board-column {
        width: 25%;
        /*background-color: dodgerblue;*/
        margin-right: 50px;
    }

    .board-colum-header {
        display: flex;
        justify-content: space-between;
        padding: 10px 10px 10px 0px;
    }
</style>