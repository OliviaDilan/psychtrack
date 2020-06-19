<script>
	export let segment;

	import '../style/nav.css';
</script>

<nav>
	<ul class="flex">
		<li  class="mr-6">
		<a class="text-gray-600 hover:text-black"  aria-current="{segment === undefined ? 'page' : undefined}" href=".">Главная</a>
		</li>
		<li  class="mr-6">
		<a class="text-gray-600 hover:text-black" aria-current="{segment === 'about' ? 'page' : undefined}" href="about">Профиль</a>
		</li>
		<li  class="mr-6">
		<a class="text-gray-600 hover:text-black" aria-current="{segment === 'profile' ? 'page' : undefined}" href="profile">Войти</a>
		</li>
	</ul>
</nav>


