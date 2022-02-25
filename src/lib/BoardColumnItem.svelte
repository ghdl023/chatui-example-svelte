<script>
    export let item;
</script>

<div class="board-column-item">
    <div>{ item.title }</div>
</div>


<style>
    .board-column-item {
        background-color: #fff;
        width:100%;
        height:150px;
        margin-bottom:15px;
        border-radius: 5px;
        box-shadow: 0 0 5px 3px #9d9d9d;
        box-sizing: border-box;
        padding:10px;
    }
</style>