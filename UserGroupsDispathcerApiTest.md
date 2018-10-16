*Test endpoint:  '/userGroups'*
========================================================================

test uses groupName 'dispatcher' , contains some comments with issues  

retrive details from userGroup : dispatcher
------------------------------------------------------------------------

details contains _links.self.href with 'groupId' value  

```
Request method:	GET
Request URI:	http://localhost:59174/userGroups?groupName=dispatcher
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
Date: Tue, 16 Oct 2018 08:52:59 GMT

{
    "groupName": "dispatcher",
    "description": "this is the dispatcher user group",
    "mappedGroupName": "cn=dispatchers, OU=groups, DC=ge, DC=com",
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
    "_links": {
        "self": {
            "href": "http://localhost:59174/v1/userGroups/2"
        },
        "userGroup": {
            "href": "http://localhost:59174/v1/userGroups/2"
        },
        "relations": {
            "href": "http://localhost:59174/v1/userGroups/2/relations"
        }
    }
}
```
add defaultAors to groupId : 2
------------------------------------------------------------------------

:exclamation: there is an inconvenience. Endpoint '/userGroups' should contains 'groupId' field, because this key value is used in further endpoints.  

```
Request method:	POST
Request URI:	http://localhost:59174/userGroups/2/defaultAors
Proxy:			<none>
Request params:	<none>
Query params:	<none>
Form params:	<none>
Path params:	<none>
Multiparts:		<none>
Headers:		Accept=*/*
				Content-Type=application/json; charset=UTF-8
Cookies:		<none>
Body:
[
    {
        "id": 1,
        "name": "wa.gordon.roarke.feeder01",
        "description": "This is feeder01",
        "shortName": "feeder01",
        "lowest": true
    },
    {
        "id": 2,
        "name": "wa.gordon.roarke.feeder02",
        "description": "This is feeder02",
        "shortName": "feeder02",
        "lowest": true
    }
]
HTTP/1.1 200 
Content-Length: 0
Date: Tue, 16 Oct 2018 08:53:02 GMT
```
get defaultAors
------------------------------------------------------------------------

check that userGroup contains modified defaultAors  

```
Request method:	GET
Request URI:	http://localhost:59174/userGroups/2/defaultAors
Proxy:			<none>
Request params:	<none>
Query params:	<none>
Form params:	<none>
Path params:	<none>
Multiparts:		<none>
Headers:		Accept=*/*
				Content-Type=application/json; charset=UTF-8
Cookies:		<none>
Body:			<none>
HTTP/1.1 200 
Content-Type: application/hal+json;charset=UTF-8
Transfer-Encoding: chunked
Date: Tue, 16 Oct 2018 08:53:02 GMT

{
    "_embedded": {
        "modelAors": [
            {
                "name": "or",
                "description": "This is the Oregon state",
                "shortName": "or",
                "lowest": false,
                "_links": {
                    "self": {
                        "href": "http://localhost:59174/v1/modelAors/24"
                    },
                    "aor": {
                        "href": "http://localhost:59174/v1/modelAors/24"
                    },
                    "sessions": {
                        "href": "http://localhost:59174/v1/modelAors/24/sessions"
                    }
                }
            },
            {
                "name": "wa.gordon.roarke.feeder02",
                "description": "This is feeder02",
                "shortName": "feeder02",
                "lowest": true,
                "_links": {
                    "self": {
                        "href": "http://localhost:59174/v1/modelAors/2"
                    },
                    "aor": {
                        "href": "http://localhost:59174/v1/modelAors/2"
                    },
                    "sessions": {
                        "href": "http://localhost:59174/v1/modelAors/2/sessions"
                    }
                }
            },
            {
                "name": "wa.gordon.roarke.feeder01",
                "description": "This is feeder01",
                "shortName": "feeder01",
                "lowest": true,
                "_links": {
                    "self": {
                        "href": "http://localhost:59174/v1/modelAors/1"
                    },
                    "aor": {
                        "href": "http://localhost:59174/v1/modelAors/1"
                    },
                    "sessions": {
                        "href": "http://localhost:59174/v1/modelAors/1/sessions"
                    }
                }
            }
        ]
    },
    "_links": {
        "self": {
            "href": "http://localhost:59174/userGroups/2/defaultAors?onlyLowestAors=false"
        }
    }
}
```
get userGroup details by groupName
------------------------------------------------------------------------

```
Request method:	GET
Request URI:	http://localhost:59174/userGroups?groupName=dispatcher
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
Date: Tue, 16 Oct 2018 08:53:02 GMT

{
    "groupName": "dispatcher",
    "description": "this is the dispatcher user group",
    "mappedGroupName": "cn=dispatchers, OU=groups, DC=ge, DC=com",
    "selectableAors": [
        {
            "name": "or",
            "description": "This is the Oregon state",
            "shortName": "or",
            "lowest": false
        },
        {
            "name": "or.setzer",
            "description": "This is the Setzer county",
            "shortName": "Setzer",
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
    "_links": {
        "self": {
            "href": "http://localhost:59174/v1/userGroups/2"
        },
        "userGroup": {
            "href": "http://localhost:59174/v1/userGroups/2"
        },
        "relations": {
            "href": "http://localhost:59174/v1/userGroups/2/relations"
        }
    }
}
```
