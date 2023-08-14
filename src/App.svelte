<script>
    import {Router,Route} from "svelte-routing";
    import Navbar from "./components/Navbar.svelte";
    import Home from "./components/Home.svelte";
    import About from "./components/About.svelte";
    import Contact from "./components/Contact.svelte";
</script>

<Navbar/>

<Router>
    <Route component={Home}/>
    <Route path="/about">
        <About />
    </Route>
    <Route path="contact">
        <Contact/>
    </Route>
</Router>