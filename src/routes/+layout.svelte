<script>
    import "../app.css";
    import Header from '$lib/components/Header.svelte';
    import Footer from '$lib/components/Footer.svelte';
</script>

<Header/>
  
  <div style="position:relative; z-index: 0; min-height: 80vh;">
  <slot/>
  </div>

<Footer/>