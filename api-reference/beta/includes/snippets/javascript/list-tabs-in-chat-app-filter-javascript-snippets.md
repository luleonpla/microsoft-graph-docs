---
description: "Automatically generated file. DO NOT MODIFY"
---

```javascript

const options = {
	authProvider,
};

const client = Client.init(options);

let res = await client.api('/chats/19:d65713bc498c4a428c71ef9353e6ce20@thread.v2/tabs')
	.version('beta')
	.filter('teamsApp/id eq 'com.microsoft.teamspace.tab.web'')
	.expand('teamsApp')
	.get();

```