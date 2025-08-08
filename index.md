<html>
	<body>
			<script type='text/javascript'>
				 window.addEventListener("onEmbeddedMessagingReady",()=>{
                    console.log("Recieved Messaging Event--- inside onEmbeddedMessagingReady");
                    var lang="English";    
                    var sapAccount = "7005201"; 
                    embeddedservice_bootstrap.prechatAPI.setHiddenPrechatFields({
                    "Language":lang,
                    "SAPAccount":sapAccount,
                    "Contact_Name_c": "pharma demo",
                    "AccountRecordType": "01236000001DnoVAAS",
                    "CaseRecordType":"0121R000000P4K7QAK",
                    "Case_Region_c": "National",
                    "Origin": "PharmaClik Chat",
                    "Status": "New",
                    "Priority": "Medium",
                    "Subject":"PharmaClik Chat",
                    "WebsiteName": "PharmaClik",
                    "CaseReason" :selectedChatTopic.reason,
                    "CaseRootCauseCategory": selectedChatTopic.cause,
                    "CaseRootCauseSubCategory": selectedChatTopic.subcause 
                    
                });
                console.log("Recieved Messaging Event--- outside onEmbeddedMessagingReady");
            });
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
