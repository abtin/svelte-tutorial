<script>
    let show = true;

    const hideAnnouncement = () => {
        show = false;
    }

    let warning = true;

    const warningFlip = () => {
        warning = !warning;
    }
</script>

{#if show}
    <div class="alert" class:warning={warning}>
        %50 off all fruits. Sign up for more fruits.
        <button on:click={warningFlip}>Flip Warning</button>
        <button on:click={hideAnnouncement}>Hide</button>
    </div>
{/if}

<style>
    .warning {
        background-color: lightpink;
        color: darkred;
    }
</style>