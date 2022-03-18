<script lang="ts" context="module">
    declare const Blockly: any;
</script>
<script lang="ts">
	import { onMount } from 'svelte';
    import '../../../scratch-blocks/dist/web/vertical';

    onMount(() => {
        Blockly.inject("scratch-blocks", {
			horizontalLayout: false,
			media: '../../../scratch-blocks/media/',
		});
    });
</script>

<div id="scratch-blocks">
    
</div>

<style lang="scss">
    #scratch-blocks {
        width: 90vw;
        height: 50vh;
    }
</style>


