<script>
    export let btnText = "Component Button";
</script>

<div>
    <span on:click>click to log</span>
    <button>{btnText}</button>
</div>

<style>
    button {
        background: #4c51bf;
        border: 1px solid #4c51bf;
        color: #fff;
    }

</style>