Testing '/userGroups' Endpoint
========================================================================
run Dummy2ApiTest on serverPort : 57594
------------------------------------------------------------------------
<pre>
Request method:	GET
Request URI:	http://localhost:57594/userGroups?groupName=operator
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
Date: Tue, 16 Oct 2018 07:45:14 GMT

{
    "groupName": "operator",
    "description": "this is the operator user group",
    "mappedGroupName": "cn=operators, OU=groups, DC=ge, DC=com",
    "selectableAors": [
        {
            "name": "wa.gordon",
            "description": "This is the Gordon county",
            "shortName": "Gordon",
            "lowest": false
        },
        {
            "name": "wa",
            "description": "This is the washington state",
            "shortName": "wa",
            "lowest": false
        }
    ],
    "defaultAors": [
        {
            "name": "wa",
            "description": "This is the washington state",
            "shortName": "wa",
            "lowest": false
        }
    ],
    "_links": {
        "self": {
            "href": "http://localhost:57594/v1/userGroups/1"
        },
        "userGroup": {
            "href": "http://localhost:57594/v1/userGroups/1"
        },
        "relations": {
            "href": "http://localhost:57594/v1/userGroups/1/relations"
        }
    }
}
</pre>
run Dummy2ApiTest part2 on serverPort : 57594
------------------------------------------------------------------------
<pre>
Request method:	GET
Request URI:	http://localhost:57594/userGroups?groupName=operator
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
Date: Tue, 16 Oct 2018 07:45:15 GMT

{
    "groupName": "operator",
    "description": "this is the operator user group",
    "mappedGroupName": "cn=operators, OU=groups, DC=ge, DC=com",
    "selectableAors": [
        {
            "name": "wa.gordon",
            "description": "This is the Gordon county",
            "shortName": "Gordon",
            "lowest": false
        },
        {
            "name": "wa",
            "description": "This is the washington state",
            "shortName": "wa",
            "lowest": false
        }
    ],
    "defaultAors": [
        {
            "name": "wa",
            "description": "This is the washington state",
            "shortName": "wa",
            "lowest": false
        }
    ],
    "_links": {
        "self": {
            "href": "http://localhost:57594/v1/userGroups/1"
        },
        "userGroup": {
            "href": "http://localhost:57594/v1/userGroups/1"
        },
        "relations": {
            "href": "http://localhost:57594/v1/userGroups/1/relations"
        }
    }
}
</pre>
run Dummy2ApiTest part2 on serverPort : 57594
------------------------------------------------------------------------
<pre>
Request method:	GET
Request URI:	http://localhost:57594/userGroups?groupName=operator
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
Date: Tue, 16 Oct 2018 07:45:15 GMT

{
    "groupName": "operator",
    "description": "this is the operator user group",
    "mappedGroupName": "cn=operators, OU=groups, DC=ge, DC=com",
    "selectableAors": [
        {
            "name": "wa.gordon",
            "description": "This is the Gordon county",
            "shortName": "Gordon",
            "lowest": false
        },
        {
            "name": "wa",
            "description": "This is the washington state",
            "shortName": "wa",
            "lowest": false
        }
    ],
    "defaultAors": [
        {
            "name": "wa",
            "description": "This is the washington state",
            "shortName": "wa",
            "lowest": false
        }
    ],
    "_links": {
        "self": {
            "href": "http://localhost:57594/v1/userGroups/1"
        },
        "userGroup": {
            "href": "http://localhost:57594/v1/userGroups/1"
        },
        "relations": {
            "href": "http://localhost:57594/v1/userGroups/1/relations"
        }
    }
}
</pre>
