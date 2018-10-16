*Test endpoint:  '/userGroups'*
========================================================================

test uses groupName 'dispatcher' , contains some comments with issues  

retrive details from userGroup : dispatcher
------------------------------------------------------------------------

<span style="color:#FF0000">there is an inconvenience: endpoint should contains groupId field, because this key value is used in further endpoints !</span> 

```
Request method:	GET
Request URI:	http://localhost:58421/userGroups?groupName=dispatcher
Proxy:			<none>
Request params:	<none>
Query params:	<none>
Form params:	<none>
Path params:	<none>
Multiparts:		<none>
Headers:		Accept=*/*
Cookies:		<none>
Body:			<none>
HTTP/1.1 200 
Content-Type: application/hal+json;charset=UTF-8
Transfer-Encoding: chunked
Date: Tue, 16 Oct 2018 08:23:05 GMT

{
    "groupName": "dispatcher",
    "description": "this is the dispatcher user group",
    "mappedGroupName": "cn=dispatchers, OU=groups, DC=ge, DC=com",
    "defaultAors": [
        {
            "name": "or",
            "description": "This is the Oregon state",
            "shortName": "or",
            "lowest": false
        },
        {
            "name": "wa.gordon.roarke.feeder02",
            "description": "This is feeder02",
            "shortName": "feeder02",
            "lowest": true
        },
        {
            "name": "wa.gordon.roarke.feeder01",
            "description": "This is feeder01",
            "shortName": "feeder01",
            "lowest": true
        }
    ],
    "selectableAors": [
        {
            "name": "or",
            "description": "This is the Oregon state",
            "shortName": "or",
            "lowest": false
        },
        {
            "name": "wa.gordon.roarke.feeder02",
            "description": "This is feeder02",
            "shortName": "feeder02",
            "lowest": true
        },
        {
            "name": "or.setzer",
            "description": "This is the Setzer county",
            "shortName": "Setzer",
            "lowest": false
        },
        {
            "name": "wa.gordon.roarke.feeder01",
            "description": "This is feeder01",
            "shortName": "feeder01",
            "lowest": true
        }
    ],
    "_links": {
        "self": {
            "href": "http://localhost:58421/v1/userGroups/2"
        },
        "userGroup": {
            "href": "http://localhost:58421/v1/userGroups/2"
        },
        "relations": {
            "href": "http://localhost:58421/v1/userGroups/2/relations"
        }
    }
}
add defaultAors to groupId : 2
------------------------------------------------------------------------

get defaultAors by groupId : 2
------------------------------------------------------------------------

```
get userGroup details by groupName
------------------------------------------------------------------------

<pre>
Request method:	GET
Request URI:	http://localhost:58421/userGroups?groupName=dispatcher
Proxy:			<none>
Request params:	<none>
Query params:	<none>
Form params:	<none>
Path params:	<none>
Multiparts:		<none>
Headers:		Accept=*/*
Cookies:		<none>
Body:			<none>
HTTP/1.1 200 
Content-Type: application/hal+json;charset=UTF-8
Transfer-Encoding: chunked
Date: Tue, 16 Oct 2018 08:23:08 GMT

{
    "groupName": "dispatcher",
    "description": "this is the dispatcher user group",
    "mappedGroupName": "cn=dispatchers, OU=groups, DC=ge, DC=com",
    "defaultAors": [
        {
            "name": "or",
            "description": "This is the Oregon state",
            "shortName": "or",
            "lowest": false
        },
        {
            "name": "wa.gordon.roarke.feeder02",
            "description": "This is feeder02",
            "shortName": "feeder02",
            "lowest": true
        },
        {
            "name": "wa.gordon.roarke.feeder01",
            "description": "This is feeder01",
            "shortName": "feeder01",
            "lowest": true
        }
    ],
    "selectableAors": [
        {
            "name": "or",
            "description": "This is the Oregon state",
            "shortName": "or",
            "lowest": false
        },
        {
            "name": "wa.gordon.roarke.feeder02",
            "description": "This is feeder02",
            "shortName": "feeder02",
            "lowest": true
        },
        {
            "name": "or.setzer",
            "description": "This is the Setzer county",
            "shortName": "Setzer",
            "lowest": false
        },
        {
            "name": "wa.gordon.roarke.feeder01",
            "description": "This is feeder01",
            "shortName": "feeder01",
            "lowest": true
        }
    ],
    "_links": {
        "self": {
            "href": "http://localhost:58421/v1/userGroups/2"
        },
        "userGroup": {
            "href": "http://localhost:58421/v1/userGroups/2"
        },
        "relations": {
            "href": "http://localhost:58421/v1/userGroups/2/relations"
        }
    }
}
</pre>
