<script>
  import logo from './assets/svelte.png'
  import Counter from './lib/Counter.svelte'
  import Header from "./lib/Header.svelte";
  import BoardColumn from "./lib/BoardColumn.svelte";
</script>

<main>
    <Header/>
    <div class="board-container">
        <BoardColumn columnName="Ready"/>
        <BoardColumn columnName="In progress"/>
        <BoardColumn columnName="Complete"/>
        <BoardColumn columnName="On hold"/>
    </div>
</main>

<style>
  body {
      background-color: rgba(0,0,0, 0.9);
      padding: 15px 5px;
  }
  .board-container {
      display:flex;
      padding: 60px 30px 0 30px;
  }
</style>
