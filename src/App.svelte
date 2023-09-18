<script>
	import { Router, Route } from 'svelte-routing';
	import Navbar from './components/Navbar.svelte';
	import Footer from './components/Footer.svelte';
	import Home from './routes/Home.svelte';
	import Logbook from './routes/Logbook.svelte';
	import Login from './routes/Login.svelte';
	import Register from './routes/Register.svelte';
  </script>
  
  <Navbar />
  <Router>
	<Route path="/" component={Home} />
	<Route path="/logbook" component={Logbook} />
	<Route path="/login" component={Login} />
	<Route path="/register" component={Register} />
  </Router>  
  <Footer />
  