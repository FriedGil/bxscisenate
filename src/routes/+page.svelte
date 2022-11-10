
<script>
    import { Text, Center } from '@svelteuidev/core';
</script>

<style>
    .full{
        min-height: 100vh;
        min-width: 100%;
        float:left;

    }
    .full.first{
        background-color: #FDFDBD;
    }

    .full.second{
        background-color: #C8FFD4;
    }

    .full.third {
        background-color: #B8E8FC;
    }
    html {
    scroll-behavior: smooth;
    margin: 0;
    }
</style>



<html lang="en" style="margin:0;">
    <div id="about" class="full first" style>
        <Center>
            <Text>
                About
            </Text>
        </Center>

    </div>
    
    
    <div id="resources" class="full second">
    
        <Center>
            <Text>
                Resources
            </Text>
        </Center>

    </div>

    <div id="contact" class="full third">
    
        <Center>
            <Text>
                Contact
            </Text>
        </Center>
    </div>

    
</html>
