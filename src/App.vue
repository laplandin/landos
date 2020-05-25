<template>
	<div id="app">
		<Index />
		<Beautiful />
		<News />
		<Price />
		<GetStarted />
		<Form />
		<Map />
		<Footer />
	</div>
</template>

<script>
    import HelloWorld from './components/HelloWorld.vue'
    import Index from './components/index.vue'
    import Beautiful from './components/beautiful.vue';
    import News from './components/News.vue';
    import Price from './components/pricing.vue';
    import GetStarted from './components/get-started.vue';
    import Form from './components/form.vue';
    import Map from './components/Map.vue';
    import Footer from './components/footer.vue';

    export default {
        name: 'App',
        components: {
            HelloWorld,
            Index,
            Beautiful,
            News,
            Price,
            GetStarted,
            Form,
            Map,
            Footer,
        }
    }
</script>

<style>
	body {
		overflow-x: hidden;
	}
	#app {
		font-family: Avenir, Helvetica, Arial, sans-serif;
		-webkit-font-smoothing: antialiased;
		-moz-osx-font-smoothing: grayscale;
		text-align: center;
		color: #2c3e50;
	}
</style>
