
<script>
	import { Burger, Space } from '@svelteuidev/core';

    let opened = false;
</script>



    <div style="background-color: lime; display: flex;">
        <Space w={30}/>
        <Burger
        {opened}
        on:click={() => (opened = !opened)}
        /> 
    </div>    
