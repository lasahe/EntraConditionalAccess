{
    "displayName": "CA03-AllApps-RequireMFA-AllUsers-When-HighMediumRisk",
    "state": "enabledForReportingButNotEnforced",
    "conditions": {
        "clientAppTypes": [
            "All"
        ],
        "applications": {
            "includeApplications": [
                "All"
            ]
        },
        "users": {
            "includeUsers": [
                "All"
            ],
            "excludeUsers": [
                "197b6aa6-8d55-4893-993a-f06040b6626e"
            ],
            "excludeGuestsOrExternalUsers": {
                "guestOrExternalUserTypes": "internalGuest,b2bCollaborationGuest,b2bCollaborationMember,b2bDirectConnectUser,otherExternalUser,serviceProvider",
                "externalTenants": {
                    "@odata.type": "#microsoft.graph.conditionalAccessAllExternalTenants",
                    "membershipKind": "all"
                }
            }
        },
        "userRiskLevels": [],
        "signInRiskLevels": [
            "high",
            "medium"
        ]
    },
    "grantControls": {
        "operator": "OR",
        "builtInControls": [
            "mfa"
        ]
    },
    "sessionControls": {
                "disableResilienceDefaults": null,
                "applicationEnforcedRestrictions": null,
                "cloudAppSecurity": null,
                "persistentBrowser": null,
                "signInFrequency": {
                    "value": null,
                    "type": null,
                    "authenticationType": "primaryAndSecondaryAuthentication",
                    "frequencyInterval": "everyTime",
                    "isEnabled": true
                }
    }
}
