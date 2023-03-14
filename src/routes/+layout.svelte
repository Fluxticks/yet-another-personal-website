<script>
	import '../app.postcss';
	import { siteDarkMode } from '../stores.js';

	siteDarkMode.subscribe((value) => {
		const classList = document.documentElement.classList;
		if (value) {
			if (!classList.contains('dark')) document.documentElement.classList.add('dark');
		} else {
			if (classList.contains('dark')) document.documentElement.classList.remove('dark');
		}
	});
</script>

<slot />
