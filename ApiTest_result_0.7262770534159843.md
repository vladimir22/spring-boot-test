Testing '/userGroups' Endpoint
========================================================================

tests for '/userGroups' endpoints  

retrive userGroup data by groupName
------------------------------------------------------------------------

server runs on serverPort: 57802  

<pre>
Request method:	GET
Request URI:	http://localhost:57802/userGroups?groupName=operator
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
Date: Tue, 16 Oct 2018 07:54:43 GMT

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
            "href": "http://localhost:57802/v1/userGroups/1"
        },
        "userGroup": {
            "href": "http://localhost:57802/v1/userGroups/1"
        },
        "relations": {
            "href": "http://localhost:57802/v1/userGroups/1/relations"
        }
    }
}
</pre>
run Dummy2ApiTest part2 on serverPort : 57802
------------------------------------------------------------------------

<pre>
Request method:	GET
Request URI:	http://localhost:57802/userGroups?groupName=operator
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
Date: Tue, 16 Oct 2018 07:54:44 GMT

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
            "href": "http://localhost:57802/v1/userGroups/1"
        },
        "userGroup": {
            "href": "http://localhost:57802/v1/userGroups/1"
        },
        "relations": {
            "href": "http://localhost:57802/v1/userGroups/1/relations"
        }
    }
}
</pre>
run Dummy2ApiTest part2 on serverPort : 57802
------------------------------------------------------------------------

<pre>
Request method:	GET
Request URI:	http://localhost:57802/userGroups?groupName=operator
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
Date: Tue, 16 Oct 2018 07:54:44 GMT

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
            "href": "http://localhost:57802/v1/userGroups/1"
        },
        "userGroup": {
            "href": "http://localhost:57802/v1/userGroups/1"
        },
        "relations": {
            "href": "http://localhost:57802/v1/userGroups/1/relations"
        }
    }
}
</pre>
