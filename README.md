# svelte-chess

Svelte chess component that combines chess.js and chessground for a fully playable chessboard.

Alpha, though all methods listed here are implemented.

## Usage

Create a playable chessboard:

    <script>
        import {Chess} from 'svelte-chess';
    </script>    

    <Chess />

Example accessing the API for undo/restart buttons:

    <script>
        import {Chess} from 'svelte-chess';
        let chessApi;
    </script>    

    <Chess bind:api={chessApi}/>

    <button on:click={()=>chessApi.resetBoard()}>Restart</button>
    <button on:click={()=>chessApi.undoLastMove()}>Undo</button>

## API

* getPossibleMoves
* getFen
* move
* resetBoard
* undoLastMove
* toggleOrientation
* getTurnColor
* getMoveNumber
* getHistory

