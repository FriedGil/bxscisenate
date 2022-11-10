
<script>
    import { typewriter } from '@svelteuidev/motion';
    import Navbar from '../lib/Navbar.svelte';
</script>

<style>
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }
    .full{
        min-height: 100vh;
        min-width: 100%;
        animation: fadeIn 1s;
        animation-delay: 1s;
        animation-fill-mode: forwards;
        opacity: 0;
        float:left;


    }
    .full.first{
        background-color: lime;
    }

    .full.second{
        background-color: limegreen;
    }
</style>

<Navbar/>

<body style="margin:0;">
    <div class="full first" style>
        <p></p>
    </div>
    
    
    <div class="full second">
    
        <p></p>
    </div>
    
</body>
