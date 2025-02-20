<script>
    let { children, ...props } = $props();
</script>

<button {...props}>{@render children()}</button>

<style>
    button {
        padding: 0.5rem 1rem;
        font-size: 1rem;
        font-weight: 700;
        color: white;
        background-color: black;
        border: none;
        border-radius: 0.25rem;
        cursor: pointer;
        text-transform: uppercase;
        transition: all 0.3s;
    }

    button:hover {
        background-color: white;
        color: black;
    }
</style>