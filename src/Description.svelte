<script>
    let count = 0;
    $: doubleCount = count * 2 ;

    $: switch (count) {
            case 11:
                alert("count is dangerously high!");
                count = 0;
                break;
        }

    function clickButton() {
        count++;
    }
</script>

<p>Count: {count}, double: {doubleCount}</p>
<button on:click={clickButton}> Click </button>
