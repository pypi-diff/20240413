# Comparing `tmp/powerhub-2.0.7.tar.gz` & `tmp/powerhub-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "powerhub-2.0.7.tar", last modified: Sun Feb  4 13:54:31 2024, max compression
+gzip compressed data, was "powerhub-2.0.8.tar", last modified: Sat Apr 13 13:22:12 2024, max compression
```

## Comparing `powerhub-2.0.7.tar` & `powerhub-2.0.8.tar`

### file list

```diff
@@ -1,326 +1,326 @@
-drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2024-02-04 13:54:31.741533 powerhub-2.0.7/
--rw-r--r--   0 adrian    (1000) adrian    (1000)     5092 2024-02-04 13:53:43.000000 powerhub-2.0.7/CHANGELOG.md
--rw-r--r--   0 adrian    (1000) adrian    (1000)     1076 2023-10-30 17:38:30.000000 powerhub-2.0.7/LICENSE
--rw-r--r--   0 adrian    (1000) adrian    (1000)      111 2023-10-30 17:38:30.000000 powerhub-2.0.7/MANIFEST.in
--rw-r--r--   0 adrian    (1000) adrian    (1000)     1478 2023-10-30 17:38:30.000000 powerhub-2.0.7/Makefile
--rw-r--r--   0 adrian    (1000) adrian    (1000)     4743 2024-02-04 13:54:31.741533 powerhub-2.0.7/PKG-INFO
--rw-r--r--   0 adrian    (1000) adrian    (1000)     3007 2023-10-30 17:38:30.000000 powerhub-2.0.7/README.md
-drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2024-02-04 13:54:31.593536 powerhub-2.0.7/powerhub/
--rw-r--r--   0 adrian    (1000) adrian    (1000)       92 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/__init__.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)      875 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/__main__.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     7822 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/app.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     3654 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/args.py
-drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2024-02-04 13:54:31.713533 powerhub-2.0.7/powerhub/decoy/
--rw-r--r--   0 adrian    (1000) adrian    (1000)    24593 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/Generic.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)     1162 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/LICENSE
--rw-r--r--   0 adrian    (1000) adrian    (1000)     7970 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/M365DSCAgent.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)     8071 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/M365DSCCheckProperties.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    33091 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/M365DSCDocGenerator.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)     1874 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/M365DSCEmojis.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)      547 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/M365DSCErrorHandler.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)     8233 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/M365DSCExoResourceUtils.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    22451 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/M365DSCLogEngine.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    61996 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/M365DSCPermissions.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    45007 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/M365DSCReport.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    97789 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/M365DSCResourceGenerator.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    35156 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/M365DSCReverse.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)     2811 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/M365DSCStringEncoding.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    10325 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/M365DSCStubsUtility.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    11773 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/M365DSCTelemetryEngine.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)   125620 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/M365DSCUtil.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    59015 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_AADAdministrativeUnit.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    33241 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_AADApplication.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    19918 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_AADAuthorizationPolicy.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    61300 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_AADConditionalAccessPolicy.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    51848 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_AADEntitlementManagementAccessPackage.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    14206 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_AADEntitlementManagementAccessPackageCatalog.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    42402 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_AADEntitlementManagementAccessPackageCatalogResource.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    41336 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_AADGroup.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    14344 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_AADGroupLifecyclePolicy.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    11960 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_AADGroupsNamingPolicy.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    16053 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_AADGroupsSettings.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    16835 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_AADNamedLocationPolicy.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    14447 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_AADRoleDefinition.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    57465 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_AADRoleSetting.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)     9745 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_AADSecurityDefaults.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    16036 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_AADServicePrincipal.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    11579 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_AADTenantDetails.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    12830 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_AADTokenLifetimePolicy.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    25842 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_AADUser.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    12566 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_EXOAcceptedDomain.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    13843 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_EXOActiveSyncDeviceAccessRule.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    13508 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_EXOAddressBookPolicy.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    24147 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_EXOAddressList.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    26661 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_EXOAntiPhishPolicy.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    18087 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_EXOAntiPhishRule.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    15251 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_EXOApplicationAccessPolicy.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    13386 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_EXOAtpPolicyForO365.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    17639 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_EXOAuthenticationPolicy.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    11722 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_EXOAuthenticationPolicyAssignment.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    17222 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_EXOAvailabilityAddressSpace.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    11826 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_EXOAvailabilityConfig.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    12741 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_EXOCASMailboxPlan.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    22378 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_EXOCASMailboxSettings.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    20387 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_EXOClientAccessRule.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    14982 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_EXODataClassification.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    14274 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_EXODataEncryptionPolicy.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    19380 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_EXODistributionGroup.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    14226 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_EXODkimSigningConfig.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    15073 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_EXOEmailAddressPolicy.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    23513 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_EXOGlobalAddressList.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    15516 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_EXOHostedConnectionFilterPolicy.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    41136 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_EXOHostedContentFilterPolicy.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    17519 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_EXOHostedContentFilterRule.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    17151 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_EXOHostedOutboundSpamFilterPolicy.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    17860 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_EXOHostedOutboundSpamFilterRule.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    16739 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_EXOIRMConfiguration.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    18209 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_EXOInboundConnector.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    13874 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_EXOIntraOrganizationConnector.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    13392 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_EXOJournalRule.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    17480 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_EXOMailContact.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    13629 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_EXOMailTips.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    13725 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_EXOMailboxPlan.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    10663 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_EXOMailboxSettings.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    23980 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_EXOMalwareFilterPolicy.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    15808 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_EXOMalwareFilterRule.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    12774 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_EXOManagementRole.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    17955 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_EXOManagementRoleAssignment.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    16038 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_EXOMessageClassification.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    37293 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_EXOMobileDeviceMailboxPolicy.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    15818 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_EXOOMEConfiguration.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    14032 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_EXOOfflineAddressBook.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    15127 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_EXOOnPremisesOrganization.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    52779 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_EXOOrganizationConfig.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    22837 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_EXOOrganizationRelationship.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    18462 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_EXOOutboundConnector.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    44206 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_EXOOwaMailboxPolicy.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    14705 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_EXOPartnerApplication.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    11721 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_EXOPerimeterConfiguration.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    12699 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_EXOPolicyTipConfig.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    18285 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_EXOQuarantinePolicy.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    20905 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_EXORemoteDomain.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    11719 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_EXOResourceConfiguration.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    14800 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_EXORoleAssignmentPolicy.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    17574 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_EXOSafeAttachmentPolicy.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    17383 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_EXOSafeAttachmentRule.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    20120 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_EXOSafeLinksPolicy.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    16493 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_EXOSafeLinksRule.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    16891 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_EXOSharedMailbox.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    12849 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_EXOSharingPolicy.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    19591 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_EXOTransportConfig.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    78785 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_EXOTransportRule.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    45034 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_IntuneASRRulesPolicyWindows10.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    73682 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_IntuneAntivirusPolicyWindows10SettingCatalog.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    34659 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_IntuneAppConfigurationPolicy.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    42057 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_IntuneAppProtectionPolicyAndroid.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    39934 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_IntuneAppProtectionPolicyiOS.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    50087 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_IntuneApplicationControlPolicyWindows10.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    71885 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_IntuneAttackSurfaceReductionRulesPolicyWindows10ConfigManager.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    13713 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_IntuneDeviceAndAppManagementAssignmentFilter.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    11071 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_IntuneDeviceCategory.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    45810 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_IntuneDeviceCompliancePolicyAndroid.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    41467 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_IntuneDeviceCompliancePolicyAndroidDeviceOwner.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    45188 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_IntuneDeviceCompliancePolicyAndroidWorkProfile.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    42413 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_IntuneDeviceCompliancePolicyMacOS.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    38478 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_IntuneDeviceCompliancePolicyWindows10.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    47363 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_IntuneDeviceCompliancePolicyiOs.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    65930 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_IntuneDeviceConfigurationPolicyAndroidDeviceAdministrator.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)   113374 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_IntuneDeviceConfigurationPolicyAndroidDeviceOwner.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    45782 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_IntuneDeviceConfigurationPolicyAndroidOpenSourceProject.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    54588 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_IntuneDeviceConfigurationPolicyAndroidWorkProfile.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    67024 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_IntuneDeviceConfigurationPolicyMacOS.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)   122984 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_IntuneDeviceConfigurationPolicyWindows10.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)   120587 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_IntuneDeviceConfigurationPolicyiOS.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    12466 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_IntuneDeviceEnrollmentLimitRestriction.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    21323 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_IntuneDeviceEnrollmentPlatformRestriction.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    52448 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_IntuneExploitProtectionPolicyWindows10SettingCatalog.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    21689 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_IntuneRoleAssignment.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    17347 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_IntuneRoleDefinition.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    59967 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_IntuneSettingCatalogASRRulesPolicyWindows10.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    41218 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_IntuneWiFiConfigurationPolicyAndroidDeviceAdministrator.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    43861 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_IntuneWifiConfigurationPolicyAndroidEntrepriseDeviceOwner.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    41241 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_IntuneWifiConfigurationPolicyAndroidEntrepriseWorkProfile.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    41234 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_IntuneWifiConfigurationPolicyAndroidForWork.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    41924 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_IntuneWifiConfigurationPolicyAndroidOpenSourceProject.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    43647 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_IntuneWifiConfigurationPolicyIOS.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    43236 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_IntuneWifiConfigurationPolicyMacOS.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    44533 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_IntuneWifiConfigurationPolicyWindows10.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    10692 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_O365AdminAuditLogConfig.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    20961 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_O365Group.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)     8581 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_O365OrgCustomizationSetting.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    21315 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_ODSettings.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    10326 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_PPPowerAppsEnvironment.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    22686 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_PPTenantIsolationSettings.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    13885 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_PPTenantSettings.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    12388 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_PlannerBucket.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    13639 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_PlannerPlan.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    26083 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_PlannerTask.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)     9636 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_SCAuditConfigurationPolicy.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    24432 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_SCAutoSensitivityLabelPolicy.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    51985 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_SCAutoSensitivityLabelRule.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    13255 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_SCCaseHoldPolicy.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    10064 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_SCCaseHoldRule.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    10763 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_SCComplianceCase.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    14193 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_SCComplianceSearch.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    19723 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_SCComplianceSearchAction.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    18037 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_SCComplianceTag.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    20090 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_SCDLPCompliancePolicy.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    47402 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_SCDLPComplianceRule.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)     9275 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_SCDeviceConditionalAccessPolicy.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)     9210 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_SCDeviceConfigurationPolicy.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)     8761 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_SCFilePlanPropertyAuthority.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)     8747 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_SCFilePlanPropertyCategory.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)     9424 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_SCFilePlanPropertyCitation.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)     8767 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_SCFilePlanPropertyDepartment.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)     8760 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_SCFilePlanPropertyReferenceId.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)     9761 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_SCFilePlanPropertySubCategory.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    26116 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_SCLabelPolicy.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    17734 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_SCProtectionAlert.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    35730 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_SCRetentionCompliancePolicy.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    16260 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_SCRetentionComplianceRule.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)     8998 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_SCRetentionEventType.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    38784 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_SCSensitivityLabel.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    10081 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_SCSupervisoryReviewPolicy.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)     9484 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_SCSupervisoryReviewRule.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    14810 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_SPOAccessControlSettings.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    13938 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_SPOApp.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    11215 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_SPOBrowserIdleSignout.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    10795 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_SPOHomeSite.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    20560 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_SPOHubSite.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    15622 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_SPOOrgAssetsLibrary.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    20163 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_SPOPropertyBag.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    33805 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_SPOSearchManagedProperty.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    21107 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_SPOSearchResultSource.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    25511 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_SPOSharingSettings.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    33664 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_SPOSite.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    12079 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_SPOSiteAuditSettings.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    15397 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_SPOSiteDesign.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    15211 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_SPOSiteDesignRights.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    19424 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_SPOSiteGroup.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    14974 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_SPOSiteScript.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    14896 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_SPOStorageEntity.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    11656 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_SPOTenantCdnEnabled.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    12872 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_SPOTenantCdnPolicy.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    20388 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_SPOTenantSettings.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    15743 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_SPOTheme.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    12214 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_SPOUserProfileProperty.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    17391 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_TeamsCallingPolicy.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    12789 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_TeamsChannel.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    19507 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_TeamsChannelTab.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    11857 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_TeamsChannelsPolicy.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    12949 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_TeamsClientConfiguration.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    11199 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_TeamsDialInConferencingTenantSettings.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    15030 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_TeamsEmergencyCallRoutingPolicy.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    12841 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_TeamsEmergencyCallingPolicy.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    10430 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_TeamsEventsPolicy.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)     9890 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_TeamsFederationConfiguration.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    11727 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_TeamsFilesPolicy.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)     7845 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_TeamsGuestCallingConfiguration.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)     8377 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_TeamsGuestMeetingConfiguration.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    10423 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_TeamsGuestMessagingConfiguration.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    13315 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_TeamsIPPhonePolicy.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)     9854 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_TeamsMeetingBroadcastConfiguration.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    11424 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_TeamsMeetingBroadcastPolicy.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    11500 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_TeamsMeetingConfiguration.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    36324 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_TeamsMeetingPolicy.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    15551 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_TeamsMessagingPolicy.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)     9061 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_TeamsOnlineVoiceUser.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    12118 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_TeamsOnlineVoicemailPolicy.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    12897 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_TeamsOnlineVoicemailUserSettings.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)     9092 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_TeamsPstnUsage.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    13401 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_TeamsShiftsPolicy.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    21209 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_TeamsTeam.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    20751 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_TeamsTenantDialPlan.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    12135 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_TeamsUpdateManagementPolicy.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)     8147 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_TeamsUpgradeConfiguration.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)     9199 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_TeamsUpgradePolicy.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    12027 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_TeamsUser.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    12142 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_TeamsUserCallingSettings.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    11954 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_TeamsVoiceRoute.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    10406 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/MSFT_TeamsVoiceRoutingPolicy.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)   889400 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/Microsoft365.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)    11985 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/PlannerTaskObject.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)     2787 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/TestHarness.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)     2173 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/decoy/UnitTestHelper.psm1
--rw-r--r--   0 adrian    (1000) adrian    (1000)     2076 2024-02-04 09:47:32.000000 powerhub-2.0.7/powerhub/dhkex.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     2108 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/directories.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)    12033 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/flask.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     8567 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/hiddenapp.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)      702 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/logging.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     5309 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/modules.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     8491 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/parameters.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     4440 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/payloads.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     1532 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/po_args.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     2393 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/repos.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     5247 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/reverseproxy.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     4040 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/sql.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)    14671 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/stager.py
-drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2024-02-04 13:54:31.585536 powerhub-2.0.7/powerhub/static/
-drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2024-02-04 13:54:31.717533 powerhub-2.0.7/powerhub/static/css/
--rw-r--r--   0 adrian    (1000) adrian    (1000)      183 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/static/css/SourceSansPro.css
--rw-r--r--   0 adrian    (1000) adrian    (1000)   189903 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/static/css/bootstrap.min.css
--rw-r--r--   0 adrian    (1000) adrian    (1000)   625953 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/static/css/bootstrap.min.css.map
--rw-r--r--   0 adrian    (1000) adrian    (1000)     1863 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/static/css/dashboard.css
-drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2024-02-04 13:54:31.729533 powerhub-2.0.7/powerhub/static/js/
--rw-r--r--   0 adrian    (1000) adrian    (1000)    78635 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/static/js/bootstrap.bundle.min.js
--rw-r--r--   0 adrian    (1000) adrian    (1000)   311949 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/static/js/bootstrap.bundle.min.js.map
--rw-r--r--   0 adrian    (1000) adrian    (1000)    58072 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/static/js/bootstrap.min.js
--rw-r--r--   0 adrian    (1000) adrian    (1000)   190253 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/static/js/bootstrap.min.js.map
--rw-r--r--   0 adrian    (1000) adrian    (1000)    65285 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/static/js/feather.min.js
--rw-r--r--   0 adrian    (1000) adrian    (1000)    45281 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/static/js/feather.min.js.map
--rw-r--r--   0 adrian    (1000) adrian    (1000)    86927 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/static/js/jquery-3.3.1.min.js
--rw-r--r--   0 adrian    (1000) adrian    (1000)   132382 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/static/js/jquery-3.3.1.min.map
--rw-r--r--   0 adrian    (1000) adrian    (1000)     4229 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/static/js/powerhub.js
--rw-r--r--   0 adrian    (1000) adrian    (1000)    61701 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/static/js/socket.io.min.js
-drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2024-02-04 13:54:31.729533 powerhub-2.0.7/powerhub/templates/
--rw-r--r--   0 adrian    (1000) adrian    (1000)     2030 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/templates/helpstrings.jinja2
-drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2024-02-04 13:54:31.733533 powerhub-2.0.7/powerhub/templates/html/
--rw-r--r--   0 adrian    (1000) adrian    (1000)     3422 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/templates/html/clipboard.html
--rw-r--r--   0 adrian    (1000) adrian    (1000)     1683 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/templates/html/fileexchange.html
-drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2024-02-04 13:54:31.733533 powerhub-2.0.7/powerhub/templates/html/hub/
--rw-r--r--   0 adrian    (1000) adrian    (1000)      438 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/templates/html/hub/download-cradle.html
--rw-r--r--   0 adrian    (1000) adrian    (1000)      343 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/templates/html/hub/modulelist.html
--rw-r--r--   0 adrian    (1000) adrian    (1000)      280 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/templates/html/hub.html
--rw-r--r--   0 adrian    (1000) adrian    (1000)     3349 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/templates/html/index.html
--rw-r--r--   0 adrian    (1000) adrian    (1000)      645 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/templates/html/list-static.html
--rw-r--r--   0 adrian    (1000) adrian    (1000)     2023 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/templates/html/modules.html
--rw-r--r--   0 adrian    (1000) adrian    (1000)      583 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/templates/html/single-toast.html
--rw-r--r--   0 adrian    (1000) adrian    (1000)      401 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/templates/html/toasts.html
--rw-r--r--   0 adrian    (1000) adrian    (1000)     2444 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/templates/macros.html
--rw-r--r--   0 adrian    (1000) adrian    (1000)      264 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/templates/macros.jinja2
-drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2024-02-04 13:54:31.733533 powerhub-2.0.7/powerhub/templates/payloads/
--rw-r--r--   0 adrian    (1000) adrian    (1000)      937 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/templates/payloads/powerhub.c
--rw-r--r--   0 adrian    (1000) adrian    (1000)     1592 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/templates/payloads/powerhub.cs
--rw-r--r--   0 adrian    (1000) adrian    (1000)     1983 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/templates/payloads/powerhub.vbs
-drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2024-02-04 13:54:31.737533 powerhub-2.0.7/powerhub/templates/powershell/
-drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2024-02-04 13:54:31.741533 powerhub-2.0.7/powerhub/templates/powershell/amsi/
--rw-r--r--   0 adrian    (1000) adrian    (1000)     1803 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/templates/powershell/amsi/adam-chester.ps1
--rw-r--r--   0 adrian    (1000) adrian    (1000)     3132 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/templates/powershell/amsi/am0nsec.ps1
--rw-r--r--   0 adrian    (1000) adrian    (1000)       81 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/templates/powershell/amsi/none.ps1
--rw-r--r--   0 adrian    (1000) adrian    (1000)     1889 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/templates/powershell/amsi/process.ps1
--rw-r--r--   0 adrian    (1000) adrian    (1000)     1385 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/templates/powershell/amsi/rasta-mouse.ps1
--rw-r--r--   0 adrian    (1000) adrian    (1000)      466 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/templates/powershell/amsi/reflection.ps1
--rw-r--r--   0 adrian    (1000) adrian    (1000)      349 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/templates/powershell/amsi/reflection2.ps1
--rw-r--r--   0 adrian    (1000) adrian    (1000)     7739 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/templates/powershell/amsi/zc00l.ps1
--rw-r--r--   0 adrian    (1000) adrian    (1000)      570 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/templates/powershell/antilogging.ps1
--rw-r--r--   0 adrian    (1000) adrian    (1000)     1758 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/templates/powershell/dh_kex.ps1
--rw-r--r--   0 adrian    (1000) adrian    (1000)     1144 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/templates/powershell/disable-logging.ps1
--rw-r--r--   0 adrian    (1000) adrian    (1000)      370 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/templates/powershell/exec_dotnet.ps1
--rw-r--r--   0 adrian    (1000) adrian    (1000)      132 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/templates/powershell/modules.csv
--rw-r--r--   0 adrian    (1000) adrian    (1000)    26354 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/templates/powershell/powerhub.ps1
--rw-r--r--   0 adrian    (1000) adrian    (1000)     2672 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/templates/powershell/rc4.ps1
--rw-r--r--   0 adrian    (1000) adrian    (1000)     2236 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/templates/powershell/stage1.ps1
--rw-r--r--   0 adrian    (1000) adrian    (1000)     2740 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/templates/powershell/stage2.ps1
--rw-r--r--   0 adrian    (1000) adrian    (1000)     5912 2024-02-04 09:47:32.000000 powerhub-2.0.7/powerhub/tools.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     1415 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/upload.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     3407 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/variables.txt
--rw-r--r--   0 adrian    (1000) adrian    (1000)     3095 2023-10-30 17:38:30.000000 powerhub-2.0.7/powerhub/webdav.py
-drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2024-02-04 13:54:31.741533 powerhub-2.0.7/powerhub.egg-info/
--rw-r--r--   0 adrian    (1000) adrian    (1000)     4743 2024-02-04 13:54:31.000000 powerhub-2.0.7/powerhub.egg-info/PKG-INFO
--rw-r--r--   0 adrian    (1000) adrian    (1000)    13916 2024-02-04 13:54:31.000000 powerhub-2.0.7/powerhub.egg-info/SOURCES.txt
--rw-r--r--   0 adrian    (1000) adrian    (1000)        1 2024-02-04 13:54:31.000000 powerhub-2.0.7/powerhub.egg-info/dependency_links.txt
--rw-r--r--   0 adrian    (1000) adrian    (1000)      104 2024-02-04 13:54:31.000000 powerhub-2.0.7/powerhub.egg-info/entry_points.txt
--rw-r--r--   0 adrian    (1000) adrian    (1000)      367 2024-02-04 13:54:31.000000 powerhub-2.0.7/powerhub.egg-info/requires.txt
--rw-r--r--   0 adrian    (1000) adrian    (1000)        9 2024-02-04 13:54:31.000000 powerhub-2.0.7/powerhub.egg-info/top_level.txt
--rw-r--r--   0 adrian    (1000) adrian    (1000)     1974 2024-02-04 13:53:43.000000 powerhub-2.0.7/pyproject.toml
--rw-r--r--   0 adrian    (1000) adrian    (1000)       38 2024-02-04 13:54:31.741533 powerhub-2.0.7/setup.cfg
+drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2024-04-13 13:22:12.170428 powerhub-2.0.8/
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     5179 2024-04-13 13:21:54.000000 powerhub-2.0.8/CHANGELOG.md
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     1076 2023-10-30 17:38:30.000000 powerhub-2.0.8/LICENSE
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      111 2023-10-30 17:38:30.000000 powerhub-2.0.8/MANIFEST.in
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     1478 2023-10-30 17:38:30.000000 powerhub-2.0.8/Makefile
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     4743 2024-04-13 13:22:12.170428 powerhub-2.0.8/PKG-INFO
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     3007 2023-10-30 17:38:30.000000 powerhub-2.0.8/README.md
+drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2024-04-13 13:22:12.110429 powerhub-2.0.8/powerhub/
+-rw-r--r--   0 adrian    (1000) adrian    (1000)       92 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/__init__.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      875 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/__main__.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     7822 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/app.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     3654 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/args.py
+drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2024-04-13 13:22:12.158428 powerhub-2.0.8/powerhub/decoy/
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    24593 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/Generic.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     1162 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/LICENSE
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     7970 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/M365DSCAgent.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     8071 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/M365DSCCheckProperties.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    33091 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/M365DSCDocGenerator.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     1874 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/M365DSCEmojis.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      547 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/M365DSCErrorHandler.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     8233 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/M365DSCExoResourceUtils.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    22451 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/M365DSCLogEngine.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    61996 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/M365DSCPermissions.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    45007 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/M365DSCReport.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    97789 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/M365DSCResourceGenerator.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    35156 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/M365DSCReverse.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     2811 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/M365DSCStringEncoding.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    10325 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/M365DSCStubsUtility.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    11773 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/M365DSCTelemetryEngine.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)   125620 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/M365DSCUtil.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    59015 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_AADAdministrativeUnit.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    33241 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_AADApplication.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    19918 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_AADAuthorizationPolicy.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    61300 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_AADConditionalAccessPolicy.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    51848 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_AADEntitlementManagementAccessPackage.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    14206 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_AADEntitlementManagementAccessPackageCatalog.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    42402 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_AADEntitlementManagementAccessPackageCatalogResource.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    41336 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_AADGroup.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    14344 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_AADGroupLifecyclePolicy.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    11960 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_AADGroupsNamingPolicy.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    16053 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_AADGroupsSettings.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    16835 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_AADNamedLocationPolicy.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    14447 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_AADRoleDefinition.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    57465 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_AADRoleSetting.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     9745 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_AADSecurityDefaults.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    16036 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_AADServicePrincipal.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    11579 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_AADTenantDetails.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    12830 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_AADTokenLifetimePolicy.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    25842 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_AADUser.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    12566 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_EXOAcceptedDomain.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    13843 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_EXOActiveSyncDeviceAccessRule.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    13508 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_EXOAddressBookPolicy.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    24147 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_EXOAddressList.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    26661 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_EXOAntiPhishPolicy.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    18087 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_EXOAntiPhishRule.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    15251 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_EXOApplicationAccessPolicy.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    13386 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_EXOAtpPolicyForO365.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    17639 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_EXOAuthenticationPolicy.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    11722 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_EXOAuthenticationPolicyAssignment.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    17222 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_EXOAvailabilityAddressSpace.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    11826 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_EXOAvailabilityConfig.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    12741 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_EXOCASMailboxPlan.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    22378 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_EXOCASMailboxSettings.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    20387 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_EXOClientAccessRule.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    14982 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_EXODataClassification.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    14274 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_EXODataEncryptionPolicy.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    19380 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_EXODistributionGroup.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    14226 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_EXODkimSigningConfig.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    15073 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_EXOEmailAddressPolicy.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    23513 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_EXOGlobalAddressList.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    15516 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_EXOHostedConnectionFilterPolicy.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    41136 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_EXOHostedContentFilterPolicy.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    17519 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_EXOHostedContentFilterRule.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    17151 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_EXOHostedOutboundSpamFilterPolicy.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    17860 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_EXOHostedOutboundSpamFilterRule.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    16739 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_EXOIRMConfiguration.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    18209 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_EXOInboundConnector.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    13874 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_EXOIntraOrganizationConnector.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    13392 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_EXOJournalRule.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    17480 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_EXOMailContact.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    13629 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_EXOMailTips.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    13725 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_EXOMailboxPlan.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    10663 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_EXOMailboxSettings.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    23980 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_EXOMalwareFilterPolicy.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    15808 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_EXOMalwareFilterRule.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    12774 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_EXOManagementRole.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    17955 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_EXOManagementRoleAssignment.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    16038 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_EXOMessageClassification.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    37293 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_EXOMobileDeviceMailboxPolicy.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    15818 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_EXOOMEConfiguration.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    14032 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_EXOOfflineAddressBook.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    15127 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_EXOOnPremisesOrganization.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    52779 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_EXOOrganizationConfig.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    22837 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_EXOOrganizationRelationship.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    18462 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_EXOOutboundConnector.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    44206 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_EXOOwaMailboxPolicy.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    14705 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_EXOPartnerApplication.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    11721 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_EXOPerimeterConfiguration.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    12699 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_EXOPolicyTipConfig.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    18285 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_EXOQuarantinePolicy.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    20905 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_EXORemoteDomain.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    11719 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_EXOResourceConfiguration.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    14800 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_EXORoleAssignmentPolicy.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    17574 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_EXOSafeAttachmentPolicy.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    17383 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_EXOSafeAttachmentRule.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    20120 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_EXOSafeLinksPolicy.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    16493 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_EXOSafeLinksRule.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    16891 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_EXOSharedMailbox.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    12849 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_EXOSharingPolicy.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    19591 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_EXOTransportConfig.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    78785 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_EXOTransportRule.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    45034 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_IntuneASRRulesPolicyWindows10.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    73682 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_IntuneAntivirusPolicyWindows10SettingCatalog.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    34659 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_IntuneAppConfigurationPolicy.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    42057 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_IntuneAppProtectionPolicyAndroid.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    39934 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_IntuneAppProtectionPolicyiOS.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    50087 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_IntuneApplicationControlPolicyWindows10.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    71885 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_IntuneAttackSurfaceReductionRulesPolicyWindows10ConfigManager.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    13713 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_IntuneDeviceAndAppManagementAssignmentFilter.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    11071 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_IntuneDeviceCategory.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    45810 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_IntuneDeviceCompliancePolicyAndroid.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    41467 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_IntuneDeviceCompliancePolicyAndroidDeviceOwner.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    45188 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_IntuneDeviceCompliancePolicyAndroidWorkProfile.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    42413 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_IntuneDeviceCompliancePolicyMacOS.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    38478 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_IntuneDeviceCompliancePolicyWindows10.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    47363 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_IntuneDeviceCompliancePolicyiOs.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    65930 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_IntuneDeviceConfigurationPolicyAndroidDeviceAdministrator.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)   113374 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_IntuneDeviceConfigurationPolicyAndroidDeviceOwner.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    45782 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_IntuneDeviceConfigurationPolicyAndroidOpenSourceProject.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    54588 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_IntuneDeviceConfigurationPolicyAndroidWorkProfile.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    67024 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_IntuneDeviceConfigurationPolicyMacOS.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)   122984 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_IntuneDeviceConfigurationPolicyWindows10.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)   120587 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_IntuneDeviceConfigurationPolicyiOS.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    12466 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_IntuneDeviceEnrollmentLimitRestriction.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    21323 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_IntuneDeviceEnrollmentPlatformRestriction.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    52448 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_IntuneExploitProtectionPolicyWindows10SettingCatalog.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    21689 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_IntuneRoleAssignment.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    17347 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_IntuneRoleDefinition.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    59967 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_IntuneSettingCatalogASRRulesPolicyWindows10.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    41218 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_IntuneWiFiConfigurationPolicyAndroidDeviceAdministrator.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    43861 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_IntuneWifiConfigurationPolicyAndroidEntrepriseDeviceOwner.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    41241 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_IntuneWifiConfigurationPolicyAndroidEntrepriseWorkProfile.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    41234 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_IntuneWifiConfigurationPolicyAndroidForWork.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    41924 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_IntuneWifiConfigurationPolicyAndroidOpenSourceProject.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    43647 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_IntuneWifiConfigurationPolicyIOS.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    43236 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_IntuneWifiConfigurationPolicyMacOS.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    44533 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_IntuneWifiConfigurationPolicyWindows10.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    10692 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_O365AdminAuditLogConfig.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    20961 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_O365Group.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     8581 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_O365OrgCustomizationSetting.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    21315 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_ODSettings.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    10326 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_PPPowerAppsEnvironment.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    22686 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_PPTenantIsolationSettings.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    13885 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_PPTenantSettings.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    12388 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_PlannerBucket.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    13639 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_PlannerPlan.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    26083 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_PlannerTask.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     9636 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_SCAuditConfigurationPolicy.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    24432 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_SCAutoSensitivityLabelPolicy.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    51985 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_SCAutoSensitivityLabelRule.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    13255 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_SCCaseHoldPolicy.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    10064 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_SCCaseHoldRule.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    10763 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_SCComplianceCase.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    14193 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_SCComplianceSearch.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    19723 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_SCComplianceSearchAction.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    18037 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_SCComplianceTag.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    20090 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_SCDLPCompliancePolicy.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    47402 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_SCDLPComplianceRule.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     9275 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_SCDeviceConditionalAccessPolicy.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     9210 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_SCDeviceConfigurationPolicy.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     8761 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_SCFilePlanPropertyAuthority.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     8747 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_SCFilePlanPropertyCategory.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     9424 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_SCFilePlanPropertyCitation.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     8767 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_SCFilePlanPropertyDepartment.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     8760 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_SCFilePlanPropertyReferenceId.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     9761 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_SCFilePlanPropertySubCategory.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    26116 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_SCLabelPolicy.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    17734 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_SCProtectionAlert.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    35730 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_SCRetentionCompliancePolicy.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    16260 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_SCRetentionComplianceRule.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     8998 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_SCRetentionEventType.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    38784 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_SCSensitivityLabel.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    10081 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_SCSupervisoryReviewPolicy.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     9484 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_SCSupervisoryReviewRule.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    14810 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_SPOAccessControlSettings.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    13938 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_SPOApp.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    11215 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_SPOBrowserIdleSignout.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    10795 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_SPOHomeSite.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    20560 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_SPOHubSite.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    15622 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_SPOOrgAssetsLibrary.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    20163 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_SPOPropertyBag.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    33805 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_SPOSearchManagedProperty.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    21107 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_SPOSearchResultSource.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    25511 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_SPOSharingSettings.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    33664 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_SPOSite.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    12079 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_SPOSiteAuditSettings.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    15397 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_SPOSiteDesign.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    15211 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_SPOSiteDesignRights.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    19424 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_SPOSiteGroup.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    14974 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_SPOSiteScript.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    14896 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_SPOStorageEntity.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    11656 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_SPOTenantCdnEnabled.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    12872 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_SPOTenantCdnPolicy.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    20388 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_SPOTenantSettings.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    15743 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_SPOTheme.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    12214 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_SPOUserProfileProperty.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    17391 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_TeamsCallingPolicy.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    12789 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_TeamsChannel.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    19507 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_TeamsChannelTab.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    11857 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_TeamsChannelsPolicy.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    12949 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_TeamsClientConfiguration.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    11199 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_TeamsDialInConferencingTenantSettings.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    15030 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_TeamsEmergencyCallRoutingPolicy.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    12841 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_TeamsEmergencyCallingPolicy.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    10430 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_TeamsEventsPolicy.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     9890 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_TeamsFederationConfiguration.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    11727 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_TeamsFilesPolicy.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     7845 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_TeamsGuestCallingConfiguration.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     8377 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_TeamsGuestMeetingConfiguration.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    10423 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_TeamsGuestMessagingConfiguration.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    13315 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_TeamsIPPhonePolicy.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     9854 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_TeamsMeetingBroadcastConfiguration.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    11424 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_TeamsMeetingBroadcastPolicy.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    11500 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_TeamsMeetingConfiguration.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    36324 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_TeamsMeetingPolicy.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    15551 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_TeamsMessagingPolicy.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     9061 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_TeamsOnlineVoiceUser.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    12118 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_TeamsOnlineVoicemailPolicy.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    12897 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_TeamsOnlineVoicemailUserSettings.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     9092 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_TeamsPstnUsage.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    13401 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_TeamsShiftsPolicy.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    21209 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_TeamsTeam.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    20751 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_TeamsTenantDialPlan.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    12135 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_TeamsUpdateManagementPolicy.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     8147 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_TeamsUpgradeConfiguration.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     9199 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_TeamsUpgradePolicy.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    12027 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_TeamsUser.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    12142 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_TeamsUserCallingSettings.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    11954 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_TeamsVoiceRoute.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    10406 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/MSFT_TeamsVoiceRoutingPolicy.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)   889400 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/Microsoft365.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    11985 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/PlannerTaskObject.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     2787 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/TestHarness.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     2173 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/decoy/UnitTestHelper.psm1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     2076 2024-02-04 09:47:32.000000 powerhub-2.0.8/powerhub/dhkex.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     2108 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/directories.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    12033 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/flask.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     8567 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/hiddenapp.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      702 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/logging.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     5309 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/modules.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     8491 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/parameters.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     4440 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/payloads.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     1532 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/po_args.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     2393 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/repos.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     5247 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/reverseproxy.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     4040 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/sql.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    14671 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/stager.py
+drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2024-04-13 13:22:12.102429 powerhub-2.0.8/powerhub/static/
+drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2024-04-13 13:22:12.162428 powerhub-2.0.8/powerhub/static/css/
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      183 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/static/css/SourceSansPro.css
+-rw-r--r--   0 adrian    (1000) adrian    (1000)   189903 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/static/css/bootstrap.min.css
+-rw-r--r--   0 adrian    (1000) adrian    (1000)   625953 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/static/css/bootstrap.min.css.map
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     1863 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/static/css/dashboard.css
+drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2024-04-13 13:22:12.162428 powerhub-2.0.8/powerhub/static/js/
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    78635 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/static/js/bootstrap.bundle.min.js
+-rw-r--r--   0 adrian    (1000) adrian    (1000)   311949 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/static/js/bootstrap.bundle.min.js.map
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    58072 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/static/js/bootstrap.min.js
+-rw-r--r--   0 adrian    (1000) adrian    (1000)   190253 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/static/js/bootstrap.min.js.map
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    65285 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/static/js/feather.min.js
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    45281 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/static/js/feather.min.js.map
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    86927 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/static/js/jquery-3.3.1.min.js
+-rw-r--r--   0 adrian    (1000) adrian    (1000)   132382 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/static/js/jquery-3.3.1.min.map
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     4229 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/static/js/powerhub.js
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    61701 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/static/js/socket.io.min.js
+drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2024-04-13 13:22:12.166428 powerhub-2.0.8/powerhub/templates/
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     2030 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/templates/helpstrings.jinja2
+drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2024-04-13 13:22:12.166428 powerhub-2.0.8/powerhub/templates/html/
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     3422 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/templates/html/clipboard.html
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     1683 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/templates/html/fileexchange.html
+drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2024-04-13 13:22:12.166428 powerhub-2.0.8/powerhub/templates/html/hub/
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      438 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/templates/html/hub/download-cradle.html
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      343 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/templates/html/hub/modulelist.html
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      280 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/templates/html/hub.html
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     3349 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/templates/html/index.html
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      645 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/templates/html/list-static.html
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     2023 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/templates/html/modules.html
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      583 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/templates/html/single-toast.html
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      401 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/templates/html/toasts.html
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     2444 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/templates/macros.html
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      264 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/templates/macros.jinja2
+drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2024-04-13 13:22:12.166428 powerhub-2.0.8/powerhub/templates/payloads/
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      937 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/templates/payloads/powerhub.c
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     1592 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/templates/payloads/powerhub.cs
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     1983 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/templates/payloads/powerhub.vbs
+drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2024-04-13 13:22:12.170428 powerhub-2.0.8/powerhub/templates/powershell/
+drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2024-04-13 13:22:12.170428 powerhub-2.0.8/powerhub/templates/powershell/amsi/
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     1803 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/templates/powershell/amsi/adam-chester.ps1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     3132 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/templates/powershell/amsi/am0nsec.ps1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)       81 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/templates/powershell/amsi/none.ps1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     1889 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/templates/powershell/amsi/process.ps1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     1385 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/templates/powershell/amsi/rasta-mouse.ps1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      466 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/templates/powershell/amsi/reflection.ps1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      349 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/templates/powershell/amsi/reflection2.ps1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     7739 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/templates/powershell/amsi/zc00l.ps1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      570 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/templates/powershell/antilogging.ps1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     1758 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/templates/powershell/dh_kex.ps1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     1144 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/templates/powershell/disable-logging.ps1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      370 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/templates/powershell/exec_dotnet.ps1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      132 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/templates/powershell/modules.csv
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    26361 2024-03-29 15:29:08.000000 powerhub-2.0.8/powerhub/templates/powershell/powerhub.ps1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     2672 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/templates/powershell/rc4.ps1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     2236 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/templates/powershell/stage1.ps1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     2740 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/templates/powershell/stage2.ps1
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     5912 2024-02-04 09:47:32.000000 powerhub-2.0.8/powerhub/tools.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     1415 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/upload.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     3407 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/variables.txt
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     3095 2023-10-30 17:38:30.000000 powerhub-2.0.8/powerhub/webdav.py
+drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2024-04-13 13:22:12.170428 powerhub-2.0.8/powerhub.egg-info/
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     4743 2024-04-13 13:22:12.000000 powerhub-2.0.8/powerhub.egg-info/PKG-INFO
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    13916 2024-04-13 13:22:12.000000 powerhub-2.0.8/powerhub.egg-info/SOURCES.txt
+-rw-r--r--   0 adrian    (1000) adrian    (1000)        1 2024-04-13 13:22:12.000000 powerhub-2.0.8/powerhub.egg-info/dependency_links.txt
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      104 2024-04-13 13:22:12.000000 powerhub-2.0.8/powerhub.egg-info/entry_points.txt
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      367 2024-04-13 13:22:12.000000 powerhub-2.0.8/powerhub.egg-info/requires.txt
+-rw-r--r--   0 adrian    (1000) adrian    (1000)        9 2024-04-13 13:22:12.000000 powerhub-2.0.8/powerhub.egg-info/top_level.txt
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     1974 2024-04-13 13:21:54.000000 powerhub-2.0.8/pyproject.toml
+-rw-r--r--   0 adrian    (1000) adrian    (1000)       38 2024-04-13 13:22:12.170428 powerhub-2.0.8/setup.cfg
```

### Comparing `powerhub-2.0.7/CHANGELOG.md` & `powerhub-2.0.8/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 Changelog
 =========
 
 All notable changes to this project will be documented in this file.
 
 ## [Unreleased]
 
+## [2.0.8] - 2024-04-13
+
+### Fixed
+
+* Fix bug that prevented loading of a lone module
+
 ## [2.0.7] - 2024-02-04
 
 ### Fixed
 
 * Establish compatibility with `cryptography` 42.0.0
 
 ## [2.0.6] - 2023-10-30
```

### Comparing `powerhub-2.0.7/LICENSE` & `powerhub-2.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/Makefile` & `powerhub-2.0.8/Makefile`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/PKG-INFO` & `powerhub-2.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: powerhub
-Version: 2.0.7
+Version: 2.0.8
 Summary: A post exploitation tool based on a web application, focusing on bypassing endpoint protection and application whitelisting
 Author-email: Adrian Vollmer <computerfluesterer@protonmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/AdrianVollmer/PowerHub
 Project-URL: Bug Tracker, https://github.com/AdrianVollmer/PowerHub/issues
 Keywords: pentest,c2,powershell,obfuscation,post-exploitation
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `powerhub-2.0.7/README.md` & `powerhub-2.0.8/README.md`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/__main__.py` & `powerhub-2.0.8/powerhub/__main__.py`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/app.py` & `powerhub-2.0.8/powerhub/app.py`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/args.py` & `powerhub-2.0.8/powerhub/args.py`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/Generic.psm1` & `powerhub-2.0.8/powerhub/decoy/Generic.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/LICENSE` & `powerhub-2.0.8/powerhub/decoy/LICENSE`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/M365DSCAgent.psm1` & `powerhub-2.0.8/powerhub/decoy/M365DSCAgent.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/M365DSCCheckProperties.psm1` & `powerhub-2.0.8/powerhub/decoy/M365DSCCheckProperties.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/M365DSCDocGenerator.psm1` & `powerhub-2.0.8/powerhub/decoy/M365DSCDocGenerator.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/M365DSCEmojis.psm1` & `powerhub-2.0.8/powerhub/decoy/M365DSCEmojis.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/M365DSCErrorHandler.psm1` & `powerhub-2.0.8/powerhub/decoy/M365DSCErrorHandler.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/M365DSCExoResourceUtils.psm1` & `powerhub-2.0.8/powerhub/decoy/M365DSCExoResourceUtils.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/M365DSCLogEngine.psm1` & `powerhub-2.0.8/powerhub/decoy/M365DSCLogEngine.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/M365DSCPermissions.psm1` & `powerhub-2.0.8/powerhub/decoy/M365DSCPermissions.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/M365DSCReport.psm1` & `powerhub-2.0.8/powerhub/decoy/M365DSCReport.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/M365DSCResourceGenerator.psm1` & `powerhub-2.0.8/powerhub/decoy/M365DSCResourceGenerator.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/M365DSCReverse.psm1` & `powerhub-2.0.8/powerhub/decoy/M365DSCReverse.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/M365DSCStringEncoding.psm1` & `powerhub-2.0.8/powerhub/decoy/M365DSCStringEncoding.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/M365DSCStubsUtility.psm1` & `powerhub-2.0.8/powerhub/decoy/M365DSCStubsUtility.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/M365DSCTelemetryEngine.psm1` & `powerhub-2.0.8/powerhub/decoy/M365DSCTelemetryEngine.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/M365DSCUtil.psm1` & `powerhub-2.0.8/powerhub/decoy/M365DSCUtil.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_AADAdministrativeUnit.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_AADAdministrativeUnit.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_AADApplication.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_AADApplication.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_AADAuthorizationPolicy.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_AADAuthorizationPolicy.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_AADConditionalAccessPolicy.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_AADConditionalAccessPolicy.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_AADEntitlementManagementAccessPackage.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_AADEntitlementManagementAccessPackage.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_AADEntitlementManagementAccessPackageCatalog.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_AADEntitlementManagementAccessPackageCatalog.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_AADEntitlementManagementAccessPackageCatalogResource.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_AADEntitlementManagementAccessPackageCatalogResource.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_AADGroup.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_AADGroup.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_AADGroupLifecyclePolicy.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_AADGroupLifecyclePolicy.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_AADGroupsNamingPolicy.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_AADGroupsNamingPolicy.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_AADGroupsSettings.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_AADGroupsSettings.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_AADNamedLocationPolicy.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_AADNamedLocationPolicy.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_AADRoleDefinition.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_AADRoleDefinition.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_AADRoleSetting.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_AADRoleSetting.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_AADSecurityDefaults.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_AADSecurityDefaults.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_AADServicePrincipal.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_AADServicePrincipal.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_AADTenantDetails.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_AADTenantDetails.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_AADTokenLifetimePolicy.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_AADTokenLifetimePolicy.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_AADUser.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_AADUser.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_EXOAcceptedDomain.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_EXOAcceptedDomain.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_EXOActiveSyncDeviceAccessRule.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_EXOActiveSyncDeviceAccessRule.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_EXOAddressBookPolicy.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_EXOAddressBookPolicy.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_EXOAddressList.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_EXOAddressList.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_EXOAntiPhishPolicy.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_EXOAntiPhishPolicy.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_EXOAntiPhishRule.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_EXOAntiPhishRule.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_EXOApplicationAccessPolicy.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_EXOApplicationAccessPolicy.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_EXOAtpPolicyForO365.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_EXOAtpPolicyForO365.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_EXOAuthenticationPolicy.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_EXOAuthenticationPolicy.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_EXOAuthenticationPolicyAssignment.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_EXOAuthenticationPolicyAssignment.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_EXOAvailabilityAddressSpace.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_EXOAvailabilityAddressSpace.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_EXOAvailabilityConfig.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_EXOAvailabilityConfig.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_EXOCASMailboxPlan.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_EXOCASMailboxPlan.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_EXOCASMailboxSettings.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_EXOCASMailboxSettings.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_EXOClientAccessRule.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_EXOClientAccessRule.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_EXODataClassification.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_EXODataClassification.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_EXODataEncryptionPolicy.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_EXODataEncryptionPolicy.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_EXODistributionGroup.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_EXODistributionGroup.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_EXODkimSigningConfig.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_EXODkimSigningConfig.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_EXOEmailAddressPolicy.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_EXOEmailAddressPolicy.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_EXOGlobalAddressList.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_EXOGlobalAddressList.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_EXOHostedConnectionFilterPolicy.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_EXOHostedConnectionFilterPolicy.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_EXOHostedContentFilterPolicy.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_EXOHostedContentFilterPolicy.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_EXOHostedContentFilterRule.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_EXOHostedContentFilterRule.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_EXOHostedOutboundSpamFilterPolicy.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_EXOHostedOutboundSpamFilterPolicy.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_EXOHostedOutboundSpamFilterRule.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_EXOHostedOutboundSpamFilterRule.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_EXOIRMConfiguration.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_EXOIRMConfiguration.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_EXOInboundConnector.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_EXOInboundConnector.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_EXOIntraOrganizationConnector.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_EXOIntraOrganizationConnector.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_EXOJournalRule.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_EXOJournalRule.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_EXOMailContact.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_EXOMailContact.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_EXOMailTips.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_EXOMailTips.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_EXOMailboxPlan.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_EXOMailboxPlan.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_EXOMailboxSettings.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_EXOMailboxSettings.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_EXOMalwareFilterPolicy.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_EXOMalwareFilterPolicy.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_EXOMalwareFilterRule.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_EXOMalwareFilterRule.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_EXOManagementRole.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_EXOManagementRole.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_EXOManagementRoleAssignment.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_EXOManagementRoleAssignment.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_EXOMessageClassification.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_EXOMessageClassification.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_EXOMobileDeviceMailboxPolicy.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_EXOMobileDeviceMailboxPolicy.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_EXOOMEConfiguration.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_EXOOMEConfiguration.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_EXOOfflineAddressBook.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_EXOOfflineAddressBook.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_EXOOnPremisesOrganization.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_EXOOnPremisesOrganization.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_EXOOrganizationConfig.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_EXOOrganizationConfig.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_EXOOrganizationRelationship.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_EXOOrganizationRelationship.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_EXOOutboundConnector.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_EXOOutboundConnector.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_EXOOwaMailboxPolicy.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_EXOOwaMailboxPolicy.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_EXOPartnerApplication.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_EXOPartnerApplication.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_EXOPerimeterConfiguration.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_EXOPerimeterConfiguration.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_EXOPolicyTipConfig.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_EXOPolicyTipConfig.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_EXOQuarantinePolicy.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_EXOQuarantinePolicy.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_EXORemoteDomain.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_EXORemoteDomain.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_EXOResourceConfiguration.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_EXOResourceConfiguration.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_EXORoleAssignmentPolicy.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_EXORoleAssignmentPolicy.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_EXOSafeAttachmentPolicy.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_EXOSafeAttachmentPolicy.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_EXOSafeAttachmentRule.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_EXOSafeAttachmentRule.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_EXOSafeLinksPolicy.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_EXOSafeLinksPolicy.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_EXOSafeLinksRule.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_EXOSafeLinksRule.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_EXOSharedMailbox.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_EXOSharedMailbox.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_EXOSharingPolicy.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_EXOSharingPolicy.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_EXOTransportConfig.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_EXOTransportConfig.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_EXOTransportRule.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_EXOTransportRule.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_IntuneASRRulesPolicyWindows10.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_IntuneASRRulesPolicyWindows10.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_IntuneAntivirusPolicyWindows10SettingCatalog.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_IntuneAntivirusPolicyWindows10SettingCatalog.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_IntuneAppConfigurationPolicy.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_IntuneAppConfigurationPolicy.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_IntuneAppProtectionPolicyAndroid.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_IntuneAppProtectionPolicyAndroid.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_IntuneAppProtectionPolicyiOS.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_IntuneAppProtectionPolicyiOS.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_IntuneApplicationControlPolicyWindows10.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_IntuneApplicationControlPolicyWindows10.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_IntuneAttackSurfaceReductionRulesPolicyWindows10ConfigManager.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_IntuneAttackSurfaceReductionRulesPolicyWindows10ConfigManager.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_IntuneDeviceAndAppManagementAssignmentFilter.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_IntuneDeviceAndAppManagementAssignmentFilter.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_IntuneDeviceCategory.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_IntuneDeviceCategory.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_IntuneDeviceCompliancePolicyAndroid.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_IntuneDeviceCompliancePolicyAndroid.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_IntuneDeviceCompliancePolicyAndroidDeviceOwner.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_IntuneDeviceCompliancePolicyAndroidDeviceOwner.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_IntuneDeviceCompliancePolicyAndroidWorkProfile.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_IntuneDeviceCompliancePolicyAndroidWorkProfile.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_IntuneDeviceCompliancePolicyMacOS.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_IntuneDeviceCompliancePolicyMacOS.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_IntuneDeviceCompliancePolicyWindows10.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_IntuneDeviceCompliancePolicyWindows10.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_IntuneDeviceCompliancePolicyiOs.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_IntuneDeviceCompliancePolicyiOs.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_IntuneDeviceConfigurationPolicyAndroidDeviceAdministrator.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_IntuneDeviceConfigurationPolicyAndroidDeviceAdministrator.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_IntuneDeviceConfigurationPolicyAndroidDeviceOwner.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_IntuneDeviceConfigurationPolicyAndroidDeviceOwner.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_IntuneDeviceConfigurationPolicyAndroidOpenSourceProject.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_IntuneDeviceConfigurationPolicyAndroidOpenSourceProject.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_IntuneDeviceConfigurationPolicyAndroidWorkProfile.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_IntuneDeviceConfigurationPolicyAndroidWorkProfile.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_IntuneDeviceConfigurationPolicyMacOS.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_IntuneDeviceConfigurationPolicyMacOS.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_IntuneDeviceConfigurationPolicyWindows10.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_IntuneDeviceConfigurationPolicyWindows10.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_IntuneDeviceConfigurationPolicyiOS.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_IntuneDeviceConfigurationPolicyiOS.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_IntuneDeviceEnrollmentLimitRestriction.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_IntuneDeviceEnrollmentLimitRestriction.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_IntuneDeviceEnrollmentPlatformRestriction.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_IntuneDeviceEnrollmentPlatformRestriction.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_IntuneExploitProtectionPolicyWindows10SettingCatalog.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_IntuneExploitProtectionPolicyWindows10SettingCatalog.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_IntuneRoleAssignment.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_IntuneRoleAssignment.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_IntuneRoleDefinition.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_IntuneRoleDefinition.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_IntuneSettingCatalogASRRulesPolicyWindows10.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_IntuneSettingCatalogASRRulesPolicyWindows10.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_IntuneWiFiConfigurationPolicyAndroidDeviceAdministrator.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_IntuneWiFiConfigurationPolicyAndroidDeviceAdministrator.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_IntuneWifiConfigurationPolicyAndroidEntrepriseDeviceOwner.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_IntuneWifiConfigurationPolicyAndroidEntrepriseDeviceOwner.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_IntuneWifiConfigurationPolicyAndroidEntrepriseWorkProfile.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_IntuneWifiConfigurationPolicyAndroidEntrepriseWorkProfile.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_IntuneWifiConfigurationPolicyAndroidForWork.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_IntuneWifiConfigurationPolicyAndroidForWork.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_IntuneWifiConfigurationPolicyAndroidOpenSourceProject.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_IntuneWifiConfigurationPolicyAndroidOpenSourceProject.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_IntuneWifiConfigurationPolicyIOS.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_IntuneWifiConfigurationPolicyIOS.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_IntuneWifiConfigurationPolicyMacOS.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_IntuneWifiConfigurationPolicyMacOS.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_IntuneWifiConfigurationPolicyWindows10.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_IntuneWifiConfigurationPolicyWindows10.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_O365AdminAuditLogConfig.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_O365AdminAuditLogConfig.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_O365Group.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_O365Group.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_O365OrgCustomizationSetting.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_O365OrgCustomizationSetting.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_ODSettings.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_ODSettings.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_PPPowerAppsEnvironment.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_PPPowerAppsEnvironment.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_PPTenantIsolationSettings.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_PPTenantIsolationSettings.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_PPTenantSettings.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_PPTenantSettings.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_PlannerBucket.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_PlannerBucket.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_PlannerPlan.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_PlannerPlan.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_PlannerTask.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_PlannerTask.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_SCAuditConfigurationPolicy.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_SCAuditConfigurationPolicy.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_SCAutoSensitivityLabelPolicy.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_SCAutoSensitivityLabelPolicy.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_SCAutoSensitivityLabelRule.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_SCAutoSensitivityLabelRule.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_SCCaseHoldPolicy.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_SCCaseHoldPolicy.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_SCCaseHoldRule.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_SCCaseHoldRule.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_SCComplianceCase.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_SCComplianceCase.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_SCComplianceSearch.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_SCComplianceSearch.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_SCComplianceSearchAction.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_SCComplianceSearchAction.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_SCComplianceTag.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_SCComplianceTag.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_SCDLPCompliancePolicy.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_SCDLPCompliancePolicy.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_SCDLPComplianceRule.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_SCDLPComplianceRule.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_SCDeviceConditionalAccessPolicy.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_SCDeviceConditionalAccessPolicy.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_SCDeviceConfigurationPolicy.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_SCDeviceConfigurationPolicy.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_SCFilePlanPropertyAuthority.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_SCFilePlanPropertyAuthority.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_SCFilePlanPropertyCategory.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_SCFilePlanPropertyCategory.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_SCFilePlanPropertyCitation.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_SCFilePlanPropertyCitation.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_SCFilePlanPropertyDepartment.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_SCFilePlanPropertyDepartment.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_SCFilePlanPropertyReferenceId.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_SCFilePlanPropertyReferenceId.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_SCFilePlanPropertySubCategory.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_SCFilePlanPropertySubCategory.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_SCLabelPolicy.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_SCLabelPolicy.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_SCProtectionAlert.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_SCProtectionAlert.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_SCRetentionCompliancePolicy.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_SCRetentionCompliancePolicy.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_SCRetentionComplianceRule.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_SCRetentionComplianceRule.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_SCRetentionEventType.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_SCRetentionEventType.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_SCSensitivityLabel.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_SCSensitivityLabel.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_SCSupervisoryReviewPolicy.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_SCSupervisoryReviewPolicy.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_SCSupervisoryReviewRule.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_SCSupervisoryReviewRule.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_SPOAccessControlSettings.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_SPOAccessControlSettings.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_SPOApp.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_SPOApp.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_SPOBrowserIdleSignout.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_SPOBrowserIdleSignout.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_SPOHomeSite.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_SPOHomeSite.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_SPOHubSite.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_SPOHubSite.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_SPOOrgAssetsLibrary.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_SPOOrgAssetsLibrary.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_SPOPropertyBag.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_SPOPropertyBag.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_SPOSearchManagedProperty.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_SPOSearchManagedProperty.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_SPOSearchResultSource.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_SPOSearchResultSource.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_SPOSharingSettings.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_SPOSharingSettings.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_SPOSite.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_SPOSite.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_SPOSiteAuditSettings.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_SPOSiteAuditSettings.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_SPOSiteDesign.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_SPOSiteDesign.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_SPOSiteDesignRights.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_SPOSiteDesignRights.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_SPOSiteGroup.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_SPOSiteGroup.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_SPOSiteScript.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_SPOSiteScript.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_SPOStorageEntity.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_SPOStorageEntity.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_SPOTenantCdnEnabled.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_SPOTenantCdnEnabled.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_SPOTenantCdnPolicy.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_SPOTenantCdnPolicy.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_SPOTenantSettings.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_SPOTenantSettings.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_SPOTheme.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_SPOTheme.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_SPOUserProfileProperty.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_SPOUserProfileProperty.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_TeamsCallingPolicy.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_TeamsCallingPolicy.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_TeamsChannel.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_TeamsChannel.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_TeamsChannelTab.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_TeamsChannelTab.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_TeamsChannelsPolicy.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_TeamsChannelsPolicy.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_TeamsClientConfiguration.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_TeamsClientConfiguration.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_TeamsDialInConferencingTenantSettings.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_TeamsDialInConferencingTenantSettings.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_TeamsEmergencyCallRoutingPolicy.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_TeamsEmergencyCallRoutingPolicy.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_TeamsEmergencyCallingPolicy.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_TeamsEmergencyCallingPolicy.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_TeamsEventsPolicy.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_TeamsEventsPolicy.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_TeamsFederationConfiguration.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_TeamsFederationConfiguration.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_TeamsFilesPolicy.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_TeamsFilesPolicy.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_TeamsGuestCallingConfiguration.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_TeamsGuestCallingConfiguration.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_TeamsGuestMeetingConfiguration.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_TeamsGuestMeetingConfiguration.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_TeamsGuestMessagingConfiguration.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_TeamsGuestMessagingConfiguration.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_TeamsIPPhonePolicy.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_TeamsIPPhonePolicy.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_TeamsMeetingBroadcastConfiguration.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_TeamsMeetingBroadcastConfiguration.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_TeamsMeetingBroadcastPolicy.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_TeamsMeetingBroadcastPolicy.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_TeamsMeetingConfiguration.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_TeamsMeetingConfiguration.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_TeamsMeetingPolicy.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_TeamsMeetingPolicy.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_TeamsMessagingPolicy.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_TeamsMessagingPolicy.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_TeamsOnlineVoiceUser.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_TeamsOnlineVoiceUser.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_TeamsOnlineVoicemailPolicy.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_TeamsOnlineVoicemailPolicy.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_TeamsOnlineVoicemailUserSettings.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_TeamsOnlineVoicemailUserSettings.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_TeamsPstnUsage.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_TeamsPstnUsage.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_TeamsShiftsPolicy.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_TeamsShiftsPolicy.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_TeamsTeam.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_TeamsTeam.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_TeamsTenantDialPlan.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_TeamsTenantDialPlan.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_TeamsUpdateManagementPolicy.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_TeamsUpdateManagementPolicy.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_TeamsUpgradeConfiguration.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_TeamsUpgradeConfiguration.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_TeamsUpgradePolicy.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_TeamsUpgradePolicy.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_TeamsUser.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_TeamsUser.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_TeamsUserCallingSettings.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_TeamsUserCallingSettings.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_TeamsVoiceRoute.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_TeamsVoiceRoute.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/MSFT_TeamsVoiceRoutingPolicy.psm1` & `powerhub-2.0.8/powerhub/decoy/MSFT_TeamsVoiceRoutingPolicy.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/Microsoft365.psm1` & `powerhub-2.0.8/powerhub/decoy/Microsoft365.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/PlannerTaskObject.psm1` & `powerhub-2.0.8/powerhub/decoy/PlannerTaskObject.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/TestHarness.psm1` & `powerhub-2.0.8/powerhub/decoy/TestHarness.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/decoy/UnitTestHelper.psm1` & `powerhub-2.0.8/powerhub/decoy/UnitTestHelper.psm1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/dhkex.py` & `powerhub-2.0.8/powerhub/dhkex.py`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/directories.py` & `powerhub-2.0.8/powerhub/directories.py`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/flask.py` & `powerhub-2.0.8/powerhub/flask.py`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/hiddenapp.py` & `powerhub-2.0.8/powerhub/hiddenapp.py`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/logging.py` & `powerhub-2.0.8/powerhub/logging.py`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/modules.py` & `powerhub-2.0.8/powerhub/modules.py`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/parameters.py` & `powerhub-2.0.8/powerhub/parameters.py`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/payloads.py` & `powerhub-2.0.8/powerhub/payloads.py`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/po_args.py` & `powerhub-2.0.8/powerhub/po_args.py`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/repos.py` & `powerhub-2.0.8/powerhub/repos.py`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/reverseproxy.py` & `powerhub-2.0.8/powerhub/reverseproxy.py`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/sql.py` & `powerhub-2.0.8/powerhub/sql.py`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/stager.py` & `powerhub-2.0.8/powerhub/stager.py`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/static/css/bootstrap.min.css` & `powerhub-2.0.8/powerhub/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/static/css/bootstrap.min.css.map` & `powerhub-2.0.8/powerhub/static/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/static/css/dashboard.css` & `powerhub-2.0.8/powerhub/static/css/dashboard.css`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/static/js/bootstrap.bundle.min.js` & `powerhub-2.0.8/powerhub/static/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/static/js/bootstrap.bundle.min.js.map` & `powerhub-2.0.8/powerhub/static/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/static/js/bootstrap.min.js` & `powerhub-2.0.8/powerhub/static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/static/js/bootstrap.min.js.map` & `powerhub-2.0.8/powerhub/static/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/static/js/feather.min.js` & `powerhub-2.0.8/powerhub/static/js/feather.min.js`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/static/js/feather.min.js.map` & `powerhub-2.0.8/powerhub/static/js/feather.min.js.map`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/static/js/jquery-3.3.1.min.js` & `powerhub-2.0.8/powerhub/static/js/jquery-3.3.1.min.js`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/static/js/jquery-3.3.1.min.map` & `powerhub-2.0.8/powerhub/static/js/jquery-3.3.1.min.map`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/static/js/powerhub.js` & `powerhub-2.0.8/powerhub/static/js/powerhub.js`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/static/js/socket.io.min.js` & `powerhub-2.0.8/powerhub/static/js/socket.io.min.js`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/templates/helpstrings.jinja2` & `powerhub-2.0.8/powerhub/templates/helpstrings.jinja2`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/templates/html/clipboard.html` & `powerhub-2.0.8/powerhub/templates/html/clipboard.html`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/templates/html/fileexchange.html` & `powerhub-2.0.8/powerhub/templates/html/fileexchange.html`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/templates/html/index.html` & `powerhub-2.0.8/powerhub/templates/html/index.html`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/templates/html/list-static.html` & `powerhub-2.0.8/powerhub/templates/html/list-static.html`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/templates/html/modules.html` & `powerhub-2.0.8/powerhub/templates/html/modules.html`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/templates/html/single-toast.html` & `powerhub-2.0.8/powerhub/templates/html/single-toast.html`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/templates/macros.html` & `powerhub-2.0.8/powerhub/templates/macros.html`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/templates/payloads/powerhub.c` & `powerhub-2.0.8/powerhub/templates/payloads/powerhub.c`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/templates/payloads/powerhub.cs` & `powerhub-2.0.8/powerhub/templates/payloads/powerhub.cs`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/templates/payloads/powerhub.vbs` & `powerhub-2.0.8/powerhub/templates/payloads/powerhub.vbs`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/templates/powershell/amsi/adam-chester.ps1` & `powerhub-2.0.8/powerhub/templates/powershell/amsi/adam-chester.ps1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/templates/powershell/amsi/am0nsec.ps1` & `powerhub-2.0.8/powerhub/templates/powershell/amsi/am0nsec.ps1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/templates/powershell/amsi/process.ps1` & `powerhub-2.0.8/powerhub/templates/powershell/amsi/process.ps1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/templates/powershell/amsi/rasta-mouse.ps1` & `powerhub-2.0.8/powerhub/templates/powershell/amsi/rasta-mouse.ps1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/templates/powershell/amsi/zc00l.ps1` & `powerhub-2.0.8/powerhub/templates/powershell/amsi/zc00l.ps1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/templates/powershell/antilogging.ps1` & `powerhub-2.0.8/powerhub/templates/powershell/antilogging.ps1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/templates/powershell/dh_kex.ps1` & `powerhub-2.0.8/powerhub/templates/powershell/dh_kex.ps1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/templates/powershell/disable-logging.ps1` & `powerhub-2.0.8/powerhub/templates/powershell/disable-logging.ps1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/templates/powershell/powerhub.ps1` & `powerhub-2.0.8/powerhub/templates/powershell/powerhub.ps1`

 * *Files 0% similar despite different names*

```diff
@@ -130,15 +130,15 @@
          [byte[]] $byteOutArray = $output.ToArray()
          $byteOutArray
     }
 }
 
 function Update-HubModules {
     Write-Verbose "Updating module list..."
-    $ModuleList = Transport-String "list" | ConvertFrom-Csv
+    [array]$ModuleList = Transport-String "list" | ConvertFrom-Csv
     $Global:PowerHubModules = $ModuleList
     foreach ($m in $PowerHubModules) {
         $m.n = [Int]($m.n)
         if ($PowerHubModulesContent.ContainsKey($m.Name)) {
             $m.Loaded = $True
         } else {
             $m.Loaded = $False
```

### Comparing `powerhub-2.0.7/powerhub/templates/powershell/rc4.ps1` & `powerhub-2.0.8/powerhub/templates/powershell/rc4.ps1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/templates/powershell/stage1.ps1` & `powerhub-2.0.8/powerhub/templates/powershell/stage1.ps1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/templates/powershell/stage2.ps1` & `powerhub-2.0.8/powerhub/templates/powershell/stage2.ps1`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/tools.py` & `powerhub-2.0.8/powerhub/tools.py`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/upload.py` & `powerhub-2.0.8/powerhub/upload.py`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/variables.txt` & `powerhub-2.0.8/powerhub/variables.txt`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub/webdav.py` & `powerhub-2.0.8/powerhub/webdav.py`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/powerhub.egg-info/PKG-INFO` & `powerhub-2.0.8/powerhub.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: powerhub
-Version: 2.0.7
+Version: 2.0.8
 Summary: A post exploitation tool based on a web application, focusing on bypassing endpoint protection and application whitelisting
 Author-email: Adrian Vollmer <computerfluesterer@protonmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/AdrianVollmer/PowerHub
 Project-URL: Bug Tracker, https://github.com/AdrianVollmer/PowerHub/issues
 Keywords: pentest,c2,powershell,obfuscation,post-exploitation
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `powerhub-2.0.7/powerhub.egg-info/SOURCES.txt` & `powerhub-2.0.8/powerhub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `powerhub-2.0.7/pyproject.toml` & `powerhub-2.0.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=45", "setuptools_scm[toml]>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "powerhub"
-version = "2.0.7"
+version = "2.0.8"
 authors = [
     {name = "Adrian Vollmer", email = "computerfluesterer@protonmail.com"},
 ]
 description = "A post exploitation tool based on a web application, focusing on bypassing endpoint protection and application whitelisting"
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["pentest", "c2", "powershell", "obfuscation", "post-exploitation"]
```

