<html>
	<body>
			<script type='text/javascript'>
	function initEmbeddedMessaging() {
		try {
			embeddedservice_bootstrap.settings.language = 'en_US'; // For example, enter 'en' or 'en-US'

			embeddedservice_bootstrap.init(
				'00DDE0000044RBg',
				'Github_Testing',
				'https://mckesson--miaw.sandbox.my.site.com/ESWGithubTesting1754639637206',
				{
					scrt2URL: 'https://mckesson--miaw.sandbox.my.salesforce-scrt.com'
				}
			);
		} catch (err) {
			console.error('Error loading Embedded Messaging: ', err);
		}
	};
</script>
<script type='text/javascript' src='https://mckesson--miaw.sandbox.my.site.com/ESWGithubTesting1754639637206/assets/js/bootstrap.min.js' onload='initEmbeddedMessaging()'></script>

	</body>
</html>
