## flowhunt@3.15.1

This generator creates TypeScript/JavaScript client that utilizes [axios](https://github.com/axios/axios). The generated Node module can be used in the following environments:

Environment
* Node.js
* Webpack
* Browserify

Language level
* ES5 - you must have a Promises/A+ library installed
* ES6

Module system
* CommonJS
* ES6 module system

It can be used in both TypeScript and JavaScript. In TypeScript, the definition will be automatically resolved via `package.json`. ([Reference](https://www.typescriptlang.org/docs/handbook/declaration-files/consumption.html))

### Building

To build and compile the typescript sources to javascript use:
```
npm install
npm run build
```

### Publishing

First build the package then run `npm publish`

### Consuming

navigate to the folder of your consuming project and run one of the following commands.

_published:_

```
npm install flowhunt@3.15.1 --save
```

_unPublished (not recommended):_

```
npm install PATH_TO_GENERATED_PACKAGE --save
```

### Documentation for API Endpoints

All URIs are relative to *https://api.flowhunt.io*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*ApiKeysApi* | [**createApiKey**](docs/ApiKeysApi.md#createapikey) | **POST** /v2/api_keys/create | Create Api Key
*ApiKeysApi* | [**deleteApiKey**](docs/ApiKeysApi.md#deleteapikey) | **DELETE** /v2/api_keys/{api_key_id} | Delete Api Key
*ApiKeysApi* | [**searchApiKey**](docs/ApiKeysApi.md#searchapikey) | **POST** /v2/api_keys/search | Search Api Key
*ApiKeysApi* | [**updateApiKey**](docs/ApiKeysApi.md#updateapikey) | **PUT** /v2/api_keys/{api_key_id} | Update Api Key
*BillingApi* | [**addAddonToSubscription**](docs/BillingApi.md#addaddontosubscription) | **POST** /v2/billing/addons/{product_id}/add | Add Addon To Subscription
*BillingApi* | [**confirmShopifySubscription**](docs/BillingApi.md#confirmshopifysubscription) | **GET** /v2/billing/shopify/confirm | Confirm Shopify Subscription
*BillingApi* | [**createChangePlanPortal**](docs/BillingApi.md#createchangeplanportal) | **POST** /v2/billing/portal/change-plan/create | Create Change Plan Portal
*BillingApi* | [**createCheckout**](docs/BillingApi.md#createcheckout) | **POST** /v2/billing/checkout/create | Create Checkout
*BillingApi* | [**createUpdateInfoPortal**](docs/BillingApi.md#createupdateinfoportal) | **POST** /v2/billing/portal/update-info/create | Create Update Info Portal
*BillingApi* | [**getPricingPlans**](docs/BillingApi.md#getpricingplans) | **GET** /v2/billing/plans | Get Pricing Plans
*BillingApi* | [**getUserPlan**](docs/BillingApi.md#getuserplan) | **GET** /v2/billing/plans/me | Get User Plan
*BillingApi* | [**stripeWebhook**](docs/BillingApi.md#stripewebhook) | **POST** /v2/billing/webhook | Stripe Webhook
*ChatbotsApi* | [**createChatbot**](docs/ChatbotsApi.md#createchatbot) | **POST** /v2/chatbots/create | Create Chatbot
*ChatbotsApi* | [**deleteChatbot**](docs/ChatbotsApi.md#deletechatbot) | **DELETE** /v2/chatbots/{chatbot_id} | Delete Chatbot
*ChatbotsApi* | [**getChatbot**](docs/ChatbotsApi.md#getchatbot) | **GET** /v2/chatbots/{chatbot_id} | Get Chatbot
*ChatbotsApi* | [**searchChatbots**](docs/ChatbotsApi.md#searchchatbots) | **POST** /v2/chatbots/ | Search Chatbots
*ChatbotsApi* | [**updateChatbot**](docs/ChatbotsApi.md#updatechatbot) | **PUT** /v2/chatbots/{chatbot_id} | Update Chatbot
*CreditsApi* | [**getCreditBalance**](docs/CreditsApi.md#getcreditbalance) | **GET** /v2/credits/balance | Get Credit Balance
*CreditsApi* | [**getWorkspaceCreditBalance**](docs/CreditsApi.md#getworkspacecreditbalance) | **GET** /v2/credits/workspace_balance | Get Workspace Credit Balance
*CreditsApi* | [**searchCreditTransactions**](docs/CreditsApi.md#searchcredittransactions) | **POST** /v2/credits/search | Search Credit Transactions
*CreditsApi* | [**searchDailyCreditTransactions**](docs/CreditsApi.md#searchdailycredittransactions) | **POST** /v2/credits/search_daily | Search Daily Credit Transactions
*DocumentsApi* | [**createDocumentCategory**](docs/DocumentsApi.md#createdocumentcategory) | **POST** /v2/documents/categories/create | Create Document Category
*DocumentsApi* | [**createFaq**](docs/DocumentsApi.md#createfaq) | **POST** /v2/documents/faqs/create | Create Faq
*DocumentsApi* | [**deleteDocument**](docs/DocumentsApi.md#deletedocument) | **DELETE** /v2/documents/{doc_id} | Delete Document
*DocumentsApi* | [**deleteDocumentCategory**](docs/DocumentsApi.md#deletedocumentcategory) | **DELETE** /v2/documents/categories/{cat_id} | Delete Document Category
*DocumentsApi* | [**deleteFaq**](docs/DocumentsApi.md#deletefaq) | **DELETE** /v2/documents/faqs/{faq_id} | Delete Faq
*DocumentsApi* | [**downloadBinaryDocument**](docs/DocumentsApi.md#downloadbinarydocument) | **GET** /v2/documents/download/binary/{doc_id} | Download Binary Document
*DocumentsApi* | [**downloadTextDocument**](docs/DocumentsApi.md#downloadtextdocument) | **GET** /v2/documents/download/text/{doc_id} | Download Text Document
*DocumentsApi* | [**importFaq**](docs/DocumentsApi.md#importfaq) | **POST** /v2/documents/faqs/import | Import Faq
*DocumentsApi* | [**searchDocumentCategories**](docs/DocumentsApi.md#searchdocumentcategories) | **POST** /v2/documents/categories/search | Search Document Categories
*DocumentsApi* | [**searchDocuments**](docs/DocumentsApi.md#searchdocuments) | **POST** /v2/documents/search | Search Documents
*DocumentsApi* | [**searchFaqs**](docs/DocumentsApi.md#searchfaqs) | **POST** /v2/documents/faqs/search | Search Faqs
*DocumentsApi* | [**updateDocument**](docs/DocumentsApi.md#updatedocument) | **PUT** /v2/documents/{doc_id} | Update Document
*DocumentsApi* | [**updateDocumentCategory**](docs/DocumentsApi.md#updatedocumentcategory) | **PUT** /v2/documents/categories/{cat_id} | Update Document Category
*DocumentsApi* | [**updateFaq**](docs/DocumentsApi.md#updatefaq) | **PUT** /v2/documents/faqs/{faq_id} | Update Faq
*DocumentsApi* | [**uploadFromUrlDocument**](docs/DocumentsApi.md#uploadfromurldocument) | **POST** /v2/documents/upload-from-url/{cat_id} | Upload From Url Document
*DocumentsApi* | [**uploadMemoryDocument**](docs/DocumentsApi.md#uploadmemorydocument) | **POST** /v2/documents/upload/{cat_id} | Upload Memory Document
*FineTuningsApi* | [**createImageFt**](docs/FineTuningsApi.md#createimageft) | **POST** /v2/photo_ai/images/ | Create Image Ft
*FineTuningsApi* | [**deleteFileFt**](docs/FineTuningsApi.md#deletefileft) | **DELETE** /v2/photo_ai/files/{file_key} | Delete File Ft
*FineTuningsApi* | [**deleteImageFt**](docs/FineTuningsApi.md#deleteimageft) | **DELETE** /v2/photo_ai/images/{ft_id} | Delete Image Ft
*FineTuningsApi* | [**generateImagePrompt**](docs/FineTuningsApi.md#generateimageprompt) | **POST** /v2/photo_ai/inference/images/generate-prompt | Generate Image Prompt
*FineTuningsApi* | [**generateImages**](docs/FineTuningsApi.md#generateimages) | **POST** /v2/photo_ai/inference/images | Generate Images
*FineTuningsApi* | [**getFileFt**](docs/FineTuningsApi.md#getfileft) | **GET** /v2/photo_ai/files/{file_key} | Get File Ft
*FineTuningsApi* | [**getInferenceResults**](docs/FineTuningsApi.md#getinferenceresults) | **GET** /v2/photo_ai/inference/results/{inference_id} | Get Inference Results
*FineTuningsApi* | [**handleReplicateWebhook**](docs/FineTuningsApi.md#handlereplicatewebhook) | **POST** /v2/photo_ai/webhooks/replicate | Handle Replicate Webhook
*FineTuningsApi* | [**searchImageFts**](docs/FineTuningsApi.md#searchimagefts) | **POST** /v2/photo_ai/images/search | Search Image Fts
*FineTuningsApi* | [**searchInferenceHistory**](docs/FineTuningsApi.md#searchinferencehistory) | **POST** /v2/photo_ai/inference/history | Search Inference History
*FineTuningsApi* | [**updateImageFt**](docs/FineTuningsApi.md#updateimageft) | **PUT** /v2/photo_ai/images/{ft_id} | Update Image Ft
*FineTuningsApi* | [**uploadImageFt**](docs/FineTuningsApi.md#uploadimageft) | **POST** /v2/photo_ai/files/{ft_type}/upload | Upload Image Ft
*FlowAssistantApi* | [**applyFlowAssistantChanges**](docs/FlowAssistantApi.md#applyflowassistantchanges) | **POST** /v2/flow_assistants/apply_changes | Apply Flow Assistant Changes
*FlowAssistantApi* | [**createFlowAssistantSession**](docs/FlowAssistantApi.md#createflowassistantsession) | **POST** /v2/flow_assistants/create | Create Flow Assistant Session
*FlowAssistantApi* | [**invokeFlowAssistantResponse**](docs/FlowAssistantApi.md#invokeflowassistantresponse) | **POST** /v2/flow_assistants/{session_id}/invoke | Invoke Flow Assistant Response
*FlowAssistantApi* | [**pollFlowAssistantResponse**](docs/FlowAssistantApi.md#pollflowassistantresponse) | **POST** /v2/flow_assistants/{session_id}/invocation_response/{from_timestamp} | Poll Flow Assistant Response
*FlowAssistantApi* | [**rejectFlowAssistantChanges**](docs/FlowAssistantApi.md#rejectflowassistantchanges) | **POST** /v2/flow_assistants/reject_changes | Reject Flow Assistant Changes
*FlowMessagesApi* | [**searchFlowMessages**](docs/FlowMessagesApi.md#searchflowmessages) | **POST** /v2/chatbots/search/{session_id} | Search Flow Messages
*FlowSessionsApi* | [**deleteChatbotSessionView**](docs/FlowSessionsApi.md#deletechatbotsessionview) | **DELETE** /v2/chatbots/sessions/{session_id} | Delete Chatbot Session View
*FlowSessionsApi* | [**getChartFeedback**](docs/FlowSessionsApi.md#getchartfeedback) | **POST** /v2/chatbots/sessions/charts | Get Chart Feedback
*FlowSessionsApi* | [**getChartSessionDuration**](docs/FlowSessionsApi.md#getchartsessionduration) | **POST** /v2/chatbots/sessions/chart_session_duration | Get Chart Session Duration
*FlowSessionsApi* | [**getChatbotSessionView**](docs/FlowSessionsApi.md#getchatbotsessionview) | **GET** /v2/chatbots/sessions/{session_id} | Get Chatbot Session View
*FlowSessionsApi* | [**getToolCallsChartFeedback**](docs/FlowSessionsApi.md#gettoolcallschartfeedback) | **POST** /v2/chatbots/sessions/chart_tool_calls | Get Tool Calls Chart Feedback
*FlowSessionsApi* | [**searchChatbotSessionsView**](docs/FlowSessionsApi.md#searchchatbotsessionsview) | **POST** /v2/chatbots/sessions/search | Search Chatbot Sessions View
*FlowSessionsApi* | [**updateChatbotSessionView**](docs/FlowSessionsApi.md#updatechatbotsessionview) | **PUT** /v2/chatbots/sessions/{session_id} | Update Chatbot Session View
*FlowWebhooksApi* | [**executeThirdPartyWebhook**](docs/FlowWebhooksApi.md#executethirdpartywebhook) | **POST** /v2/flows/webhooks/third_party_integrations/{trigger_type} | Execute Third Party Webhook
*FlowWebhooksApi* | [**executeWebhook**](docs/FlowWebhooksApi.md#executewebhook) | **POST** /v2/flows/webhooks/{chatbot_id} | Execute Webhook
*FlowWebhooksApi* | [**executeWebhookFromFlow**](docs/FlowWebhooksApi.md#executewebhookfromflow) | **POST** /v2/flows/webhooks/from_flow/{flow_id} | Execute Webhook From Flow
*FlowsApi* | [**createChatbotSession**](docs/FlowsApi.md#createchatbotsession) | **POST** /v2/flows/sessions/create | Create Chatbot Session
*FlowsApi* | [**createFlow**](docs/FlowsApi.md#createflow) | **POST** /v2/flows/create | Create Flow
*FlowsApi* | [**createFlowCategory**](docs/FlowsApi.md#createflowcategory) | **POST** /v2/flows/categories/create | Create Flow Category
*FlowsApi* | [**createFlowCron**](docs/FlowsApi.md#createflowcron) | **POST** /v2/flows/crons/create | Create Flow Cron
*FlowsApi* | [**createFlowSession**](docs/FlowsApi.md#createflowsession) | **POST** /v2/flows/sessions/from_flow/create | Create Flow Session
*FlowsApi* | [**createMessageFeedback**](docs/FlowsApi.md#createmessagefeedback) | **POST** /v2/flows/sessions/{session_id}/feedback | Create Message Feedback
*FlowsApi* | [**deleteAttachment**](docs/FlowsApi.md#deleteattachment) | **DELETE** /v2/flows/sessions/{session_id}/attachments/{file_id} | Delete Attachment
*FlowsApi* | [**deleteFlow**](docs/FlowsApi.md#deleteflow) | **DELETE** /v2/flows/{flow_id} | Delete Flow
*FlowsApi* | [**deleteFlowCategory**](docs/FlowsApi.md#deleteflowcategory) | **DELETE** /v2/flows/categories/{cat_id} | Delete Flow Category
*FlowsApi* | [**deleteFlowCron**](docs/FlowsApi.md#deleteflowcron) | **DELETE** /v2/flows/crons/{flow_id}/{cron_id} | Delete Flow Cron
*FlowsApi* | [**executeFlowCron**](docs/FlowsApi.md#executeflowcron) | **POST** /v2/flows/crons/{flow_id}/{cron_id}/execute | Execute Flow Cron
*FlowsApi* | [**generateCommitMessage**](docs/FlowsApi.md#generatecommitmessage) | **POST** /v2/flows/{flow_id}/generate-commit-msg | Generate Commit Message
*FlowsApi* | [**get**](docs/FlowsApi.md#get) | **GET** /v2/flows/{flow_id} | Get
*FlowsApi* | [**getAllComponents**](docs/FlowsApi.md#getallcomponents) | **GET** /v2/flows/components/all | Get All Components
*FlowsApi* | [**getAttachments**](docs/FlowsApi.md#getattachments) | **GET** /v2/flows/sessions/{session_id}/attachments | Get Attachments
*FlowsApi* | [**getFlowVersions**](docs/FlowsApi.md#getflowversions) | **GET** /v2/flows/{flow_id}/version_history | Get Flow Versions
*FlowsApi* | [**getInvokedFlowResults**](docs/FlowsApi.md#getinvokedflowresults) | **GET** /v2/flows/{flow_id}/{task_id} | Get Invoked Flow Results
*FlowsApi* | [**getPublicFlow**](docs/FlowsApi.md#getpublicflow) | **GET** /v2/flows/public/{flow_id} | Get Public Flow
*FlowsApi* | [**getTriggerTypes**](docs/FlowsApi.md#gettriggertypes) | **POST** /v2/flows/{flow_id}/triggers | Get Trigger Types
*FlowsApi* | [**invokeFlow**](docs/FlowsApi.md#invokeflow) | **POST** /v2/flows/{flow_id}/invoke | Invoke Flow
*FlowsApi* | [**invokeFlowResponse**](docs/FlowsApi.md#invokeflowresponse) | **POST** /v2/flows/sessions/{session_id}/invoke | Invoke Flow Response
*FlowsApi* | [**invokeFlowSingleton**](docs/FlowsApi.md#invokeflowsingleton) | **POST** /v2/flows/{flow_id}/invoke_singleton | Invoke Flow Singleton
*FlowsApi* | [**pollFlowResponse**](docs/FlowsApi.md#pollflowresponse) | **POST** /v2/flows/sessions/{session_id}/invocation_response/{from_timestamp} | Poll Flow Response
*FlowsApi* | [**publishFlow**](docs/FlowsApi.md#publishflow) | **POST** /v2/flows/{flow_id}/publish | Publish Flow
*FlowsApi* | [**restoreFlowVersion**](docs/FlowsApi.md#restoreflowversion) | **POST** /v2/flows/{flow_id}/version_history/{branch}/restore | Restore Flow Version
*FlowsApi* | [**search**](docs/FlowsApi.md#search) | **POST** /v2/flows/ | Search
*FlowsApi* | [**searchAll**](docs/FlowsApi.md#searchall) | **POST** /v2/flows/all | Search All
*FlowsApi* | [**searchFlowCategories**](docs/FlowsApi.md#searchflowcategories) | **POST** /v2/flows/categories/search | Search Flow Categories
*FlowsApi* | [**searchFlowCrons**](docs/FlowsApi.md#searchflowcrons) | **POST** /v2/flows/crons/search | Search Flow Crons
*FlowsApi* | [**updateFlow**](docs/FlowsApi.md#updateflow) | **PUT** /v2/flows/{flow_id} | Update Flow
*FlowsApi* | [**updateFlowCategory**](docs/FlowsApi.md#updateflowcategory) | **PUT** /v2/flows/categories/{cat_id} | Update Flow Category
*FlowsApi* | [**updateFlowCron**](docs/FlowsApi.md#updateflowcron) | **PUT** /v2/flows/crons/{flow_id}/{cron_id} | Update Flow Cron
*FlowsApi* | [**uploadAttachments**](docs/FlowsApi.md#uploadattachments) | **POST** /v2/flows/sessions/{session_id}/attachments | Upload Attachments
*GoogleApi* | [**getCalendars**](docs/GoogleApi.md#getcalendars) | **GET** /v2/integrations/google/calendar | Get Calendars
*GoogleApi* | [**getPickerToken**](docs/GoogleApi.md#getpickertoken) | **GET** /v2/integrations/google/picker_token | Get Picker Token
*GoogleApi* | [**getSheets**](docs/GoogleApi.md#getsheets) | **GET** /v2/integrations/google/sheets/{document_id} | Get Sheets
*GoogleAdsApi* | [**addKeywordToGroup**](docs/GoogleAdsApi.md#addkeywordtogroup) | **POST** /v2/integrations/google_ads/keyword/add_to_group | Add Keyword To Group
*GoogleAdsApi* | [**analyzeNotAssignedKeywords**](docs/GoogleAdsApi.md#analyzenotassignedkeywords) | **POST** /v2/integrations/google_ads/analyze_not_assigned_keywords | Analyze Not Assigned Keywords
*GoogleAdsApi* | [**getGoogleAdsCampaigns**](docs/GoogleAdsApi.md#getgoogleadscampaigns) | **POST** /v2/integrations/google_ads/campaigns | Get Google Ads Campaigns
*GoogleAdsApi* | [**getGoogleAdsCustomers**](docs/GoogleAdsApi.md#getgoogleadscustomers) | **POST** /v2/integrations/google_ads/customers | Get Google Ads Customers
*GoogleAdsApi* | [**getGoogleAdsGroups**](docs/GoogleAdsApi.md#getgoogleadsgroups) | **POST** /v2/integrations/google_ads/groups | Get Google Ads Groups
*GoogleAdsApi* | [**getRecommendations**](docs/GoogleAdsApi.md#getrecommendations) | **POST** /v2/integrations/google_ads/recommendations/ | Get Recommendations
*GoogleAdsApi* | [**importGoogleAdsCampaigns**](docs/GoogleAdsApi.md#importgoogleadscampaigns) | **POST** /v2/integrations/google_ads/campaigns/import | Import Google Ads Campaigns
*GoogleAdsApi* | [**importGoogleAdsCustomers**](docs/GoogleAdsApi.md#importgoogleadscustomers) | **POST** /v2/integrations/google_ads/customers/import | Import Google Ads Customers
*GoogleAdsApi* | [**importGoogleAdsGroups**](docs/GoogleAdsApi.md#importgoogleadsgroups) | **POST** /v2/integrations/google_ads/groups/import | Import Google Ads Groups
*GoogleAdsApi* | [**removeKeywordFromGroup**](docs/GoogleAdsApi.md#removekeywordfromgroup) | **POST** /v2/integrations/google_ads/keyword/remove_from_group | Remove Keyword From Group
*GoogleAdsApi* | [**updateGoogleAdsCampaign**](docs/GoogleAdsApi.md#updategoogleadscampaign) | **PUT** /v2/integrations/google_ads/campaigns/{customer_id}/{campaign_id} | Update Google Ads Campaign
*GoogleAdsApi* | [**updateGoogleAdsCustomerUpdate**](docs/GoogleAdsApi.md#updategoogleadscustomerupdate) | **PUT** /v2/integrations/google_ads/customers/{customer_id} | Update Google Ads Customer Update
*GoogleAdsApi* | [**updateGoogleAdsGroup**](docs/GoogleAdsApi.md#updategoogleadsgroup) | **PUT** /v2/integrations/google_ads/groups/{customer_id}/{campaign_id}/{group_id} | Update Google Ads Group
*HealthApi* | [**health**](docs/HealthApi.md#health) | **GET** /v2/monitoring/health/ | Health
*HubSpotApi* | [**getActors**](docs/HubSpotApi.md#getactors) | **GET** /v2/integrations/hubspot/actors/ | Get Actors
*ImagesApi* | [**convertImage**](docs/ImagesApi.md#convertimage) | **POST** /v2/images/convert | Convert Image
*ImagesApi* | [**getScreenshot**](docs/ImagesApi.md#getscreenshot) | **POST** /v2/images/screenshot | Get Screenshot
*ImagesApi* | [**optimizeImage**](docs/ImagesApi.md#optimizeimage) | **POST** /v2/images/optimize | Optimize Image
*InstagramApi* | [**getProfileInformation**](docs/InstagramApi.md#getprofileinformation) | **GET** /v2/integrations/instagram/profile_information | Get Profile Information
*IntegrationsApi* | [**createIntegration**](docs/IntegrationsApi.md#createintegration) | **POST** /v2/integrations/{slug}/integrate | Create Integration
*IntegrationsApi* | [**customerDataRequest**](docs/IntegrationsApi.md#customerdatarequest) | **POST** /v2/integrations/shopify/webhooks/customers/data_request | Customer Data Request
*IntegrationsApi* | [**customerRedact**](docs/IntegrationsApi.md#customerredact) | **POST** /v2/integrations/shopify/webhooks/customers/redact | Customer Redact
*IntegrationsApi* | [**deleteIntegration**](docs/IntegrationsApi.md#deleteintegration) | **DELETE** /v2/integrations/{slug}/{integration_id} | Delete Integration
*IntegrationsApi* | [**getActors**](docs/IntegrationsApi.md#getactors) | **GET** /v2/integrations/hubspot/actors/ | Get Actors
*IntegrationsApi* | [**getAllIntegrations**](docs/IntegrationsApi.md#getallintegrations) | **GET** /v2/integrations/all | Get All Integrations
*IntegrationsApi* | [**getCalendars**](docs/IntegrationsApi.md#getcalendars) | **GET** /v2/integrations/google/calendar | Get Calendars
*IntegrationsApi* | [**getHubspotCustomChannelConnect**](docs/IntegrationsApi.md#gethubspotcustomchannelconnect) | **GET** /v2/integrations/hubspot_custom_channel_connect | Get Hubspot Custom Channel Connect
*IntegrationsApi* | [**getIntegration**](docs/IntegrationsApi.md#getintegration) | **GET** /v2/integrations/{slug}/{integration_id} | Get Integration
*IntegrationsApi* | [**getPickerToken**](docs/IntegrationsApi.md#getpickertoken) | **GET** /v2/integrations/google/picker_token | Get Picker Token
*IntegrationsApi* | [**getProfileInformation**](docs/IntegrationsApi.md#getprofileinformation) | **GET** /v2/integrations/instagram/profile_information | Get Profile Information
*IntegrationsApi* | [**getSheets**](docs/IntegrationsApi.md#getsheets) | **GET** /v2/integrations/google/sheets/{document_id} | Get Sheets
*IntegrationsApi* | [**getShopify**](docs/IntegrationsApi.md#getshopify) | **GET** /v2/integrations/shopify/ | Get Shopify
*IntegrationsApi* | [**getSlackChannels**](docs/IntegrationsApi.md#getslackchannels) | **GET** /v2/integrations/slack/{slack_team_id}/channels | Get Slack Channels
*IntegrationsApi* | [**getSlackWorkspaces**](docs/IntegrationsApi.md#getslackworkspaces) | **GET** /v2/integrations/slack/ | Get Slack Workspaces
*IntegrationsApi* | [**getWordpressPostCategories**](docs/IntegrationsApi.md#getwordpresspostcategories) | **GET** /v2/integrations/wordpress/{integration_id}/categories | Get Wordpress Post Categories
*IntegrationsApi* | [**getWordpressPostTags**](docs/IntegrationsApi.md#getwordpressposttags) | **GET** /v2/integrations/wordpress/{integration_id}/tags | Get Wordpress Post Tags
*IntegrationsApi* | [**getWordpressSites**](docs/IntegrationsApi.md#getwordpresssites) | **GET** /v2/integrations/wordpress/sites | Get Wordpress Sites
*IntegrationsApi* | [**integrationCallback**](docs/IntegrationsApi.md#integrationcallback) | **GET** /v2/integrations/{slug}/callback | Integration Callback
*IntegrationsApi* | [**searchIntegrations**](docs/IntegrationsApi.md#searchintegrations) | **POST** /v2/integrations/{slug} | Search Integrations
*IntegrationsApi* | [**shopRedact**](docs/IntegrationsApi.md#shopredact) | **POST** /v2/integrations/shopify/webhooks/shop/redact | Shop Redact
*IntegrationsApi* | [**subscriptionCancel**](docs/IntegrationsApi.md#subscriptioncancel) | **POST** /v2/integrations/shopify/webhooks/billing/subscription_cancel | Subscription Cancel
*IntegrationsApi* | [**subscriptionUpdate**](docs/IntegrationsApi.md#subscriptionupdate) | **POST** /v2/integrations/shopify/webhooks/billing/subscription_update | Subscription Update
*IntegrationsApi* | [**updateAdminConsent**](docs/IntegrationsApi.md#updateadminconsent) | **POST** /v2/integrations/microsoft_entra_id/admin_consent | Update Admin Consent
*LogsApi* | [**searchLogs**](docs/LogsApi.md#searchlogs) | **POST** /v2/logs/search | Search logs
*MCPServersApi* | [**createMcpServer**](docs/MCPServersApi.md#createmcpserver) | **POST** /v2/mcp_servers/create | Create Mcp Server
*MCPServersApi* | [**deleteMcpServer**](docs/MCPServersApi.md#deletemcpserver) | **DELETE** /v2/mcp_servers/{mcp_server_id} | Delete Mcp Server
*MCPServersApi* | [**getAllMcpSubservers**](docs/MCPServersApi.md#getallmcpsubservers) | **GET** /v2/mcp_servers/all | Get All Mcp Subservers
*MCPServersApi* | [**getMcpServer**](docs/MCPServersApi.md#getmcpserver) | **GET** /v2/mcp_servers/{mcp_server_id} | Get Mcp Server
*MCPServersApi* | [**searchMcpServers**](docs/MCPServersApi.md#searchmcpservers) | **POST** /v2/mcp_servers/ | Search Mcp Servers
*MCPServersApi* | [**updateMcpServer**](docs/MCPServersApi.md#updatemcpserver) | **PUT** /v2/mcp_servers/{mcp_server_id} | Update Mcp Server
*MeApi* | [**getUserSettings**](docs/MeApi.md#getusersettings) | **GET** /v2/users/me/settings | Get User Settings
*MeApi* | [**updateUserSettings**](docs/MeApi.md#updateusersettings) | **PUT** /v2/users/me/settings | Update User Settings
*MediaApi* | [**getTranscript**](docs/MediaApi.md#gettranscript) | **POST** /v2/media/transcript | Get Transcript
*MediaApi* | [**getTranscriptResult**](docs/MediaApi.md#gettranscriptresult) | **POST** /v2/media/transcript_status | Get Transcript Result
*MediaApi* | [**getYoutubeTranscript**](docs/MediaApi.md#getyoutubetranscript) | **POST** /v2/media/youtube/transcript | Get Youtube Transcript
*MemoryApi* | [**createNode**](docs/MemoryApi.md#createnode) | **POST** /v2/memory/node/create | Create Node
*MemoryApi* | [**deleteNode**](docs/MemoryApi.md#deletenode) | **DELETE** /v2/memory/node/{node_id} | Delete Node
*MemoryApi* | [**getNode**](docs/MemoryApi.md#getnode) | **POST** /v2/memory/node/{node_id} | Get Node
*MemoryApi* | [**processDocuments**](docs/MemoryApi.md#processdocuments) | **POST** /v2/memory/process-documents | Process Documents
*MemoryApi* | [**searchMemoryCategories**](docs/MemoryApi.md#searchmemorycategories) | **POST** /v2/memory/search | Search Memory Categories
*MemoryApi* | [**searchMemoryNodeName**](docs/MemoryApi.md#searchmemorynodename) | **POST** /v2/memory/search_node_name | Search Memory Node Name
*MemoryApi* | [**searchMemoryNodePath**](docs/MemoryApi.md#searchmemorynodepath) | **POST** /v2/memory/search_node_path | Search Memory Node Path
*MemoryApi* | [**updateNode**](docs/MemoryApi.md#updatenode) | **PUT** /v2/memory/node/{node_id} | Update Node
*MemoryApi* | [**uploadDocument**](docs/MemoryApi.md#uploaddocument) | **POST** /v2/memory/upload/{cat_id} | Upload Document
*MicrosoftOutlookApi* | [**updateAdminConsent**](docs/MicrosoftOutlookApi.md#updateadminconsent) | **POST** /v2/integrations/microsoft_entra_id/admin_consent | Update Admin Consent
*OAuthApi* | [**oauthAuthorize**](docs/OAuthApi.md#oauthauthorize) | **GET** /v2/auth/oauth/authorize | Oauth Authorize
*OAuthApi* | [**oauthAuthorizePost**](docs/OAuthApi.md#oauthauthorizepost) | **POST** /v2/auth/oauth/authorize | Oauth Authorize Post
*OAuthApi* | [**oauthCallback**](docs/OAuthApi.md#oauthcallback) | **GET** /v2/auth/oauth/callback | Oauth Callback
*OAuthApi* | [**oauthLogin**](docs/OAuthApi.md#oauthlogin) | **GET** /v2/auth/oauth/login | Oauth Login
*OAuthApi* | [**oauthLoginGithub**](docs/OAuthApi.md#oauthlogingithub) | **GET** /v2/auth/oauth/login/github | Oauth Login Github
*OAuthApi* | [**oauthLoginGoogle**](docs/OAuthApi.md#oauthlogingoogle) | **GET** /v2/auth/oauth/login/google | Oauth Login Google
*OAuthApi* | [**oauthLoginPost**](docs/OAuthApi.md#oauthloginpost) | **POST** /v2/auth/oauth/login | Oauth Login Post
*OAuthApi* | [**oauthLoginShopify**](docs/OAuthApi.md#oauthloginshopify) | **GET** /v2/auth/oauth/login/shopify | Oauth Login Shopify
*OAuthApi* | [**oauthLogout**](docs/OAuthApi.md#oauthlogout) | **GET** /v2/auth/oauth/logout | Oauth Logout
*OAuthApi* | [**oauthRevoke**](docs/OAuthApi.md#oauthrevoke) | **POST** /v2/auth/oauth/revoke | Oauth Revoke
*OAuthApi* | [**oauthToken**](docs/OAuthApi.md#oauthtoken) | **POST** /v2/auth/oauth/token | Oauth Token
*OAuthApi* | [**oauthUserinfo**](docs/OAuthApi.md#oauthuserinfo) | **GET** /v2/auth/oauth/userinfo | Oauth Userinfo
*OAuthApi* | [**samlCallback**](docs/OAuthApi.md#samlcallback) | **POST** /v2/auth/oauth/callback/saml/{random_id} | Saml Callback
*ObservabilityDriverApi* | [**activateLangfuseObservabilityDriver**](docs/ObservabilityDriverApi.md#activatelangfuseobservabilitydriver) | **POST** /v2/observability_driver/langfuse | Activate Langfuse Observability Driver
*ObservabilityDriverApi* | [**activatePowerBiObservabilityDriver**](docs/ObservabilityDriverApi.md#activatepowerbiobservabilitydriver) | **POST** /v2/observability_driver/power_bi | Activate Power Bi Observability Driver
*ObservabilityDriverApi* | [**createPowerBiPushDataset**](docs/ObservabilityDriverApi.md#createpowerbipushdataset) | **POST** /v2/observability_driver/power_bi/push_dataset | Create Power Bi Push Dataset
*ObservabilityDriverApi* | [**deleteObservabilityDriver**](docs/ObservabilityDriverApi.md#deleteobservabilitydriver) | **DELETE** /v2/observability_driver/{driver_type} | Delete Observability Driver
*ObservabilityDriverApi* | [**getObservabilityDriver**](docs/ObservabilityDriverApi.md#getobservabilitydriver) | **GET** /v2/observability_driver/{driver_type} | Get Observability Driver
*ObservabilityDriverApi* | [**getObservabilityDriverWorkspace**](docs/ObservabilityDriverApi.md#getobservabilitydriverworkspace) | **POST** /v2/observability_driver/ | Get Observability Driver Workspace
*ObservabilityDriverApi* | [**listPowerBiDatasets**](docs/ObservabilityDriverApi.md#listpowerbidatasets) | **POST** /v2/observability_driver/power_bi/datasets | List Power Bi Datasets
*ObservabilityDriverApi* | [**listPowerBiTables**](docs/ObservabilityDriverApi.md#listpowerbitables) | **POST** /v2/observability_driver/power_bi/tables | List Power Bi Tables
*ObservabilityDriverApi* | [**listPowerBiWorkspaces**](docs/ObservabilityDriverApi.md#listpowerbiworkspaces) | **GET** /v2/observability_driver/power_bi/workspaces | List Power Bi Workspaces
*ObservabilityDriverApi* | [**updateLangfuseObservabilityDriver**](docs/ObservabilityDriverApi.md#updatelangfuseobservabilitydriver) | **PUT** /v2/observability_driver/langfuse | Update Langfuse Observability Driver
*ObservabilityDriverApi* | [**updatePowerBiObservabilityDriver**](docs/ObservabilityDriverApi.md#updatepowerbiobservabilitydriver) | **PUT** /v2/observability_driver/power_bi | Update Power Bi Observability Driver
*ObservabilityDriverApi* | [**validatePushDatasetTable**](docs/ObservabilityDriverApi.md#validatepushdatasettable) | **POST** /v2/observability_driver/power_bi/validate_push_dataset | Validate Push Dataset Table
*PhotoAIApi* | [**explore**](docs/PhotoAIApi.md#explore) | **GET** /v2/photo_ai/public/explore | Explore
*PhotoAIApi* | [**getEffects**](docs/PhotoAIApi.md#geteffects) | **GET** /v2/photo_ai/public/effects | Get Effects
*PhotoAIApi* | [**getStyles**](docs/PhotoAIApi.md#getstyles) | **GET** /v2/photo_ai/public/styles | Get Styles
*PhotoAIApi* | [**getTemplates**](docs/PhotoAIApi.md#gettemplates) | **GET** /v2/photo_ai/public/templates | Get Templates
*PromptsApi* | [**createPrompt**](docs/PromptsApi.md#createprompt) | **POST** /v2/prompts/create | Create Prompt
*PromptsApi* | [**createPromptCategory**](docs/PromptsApi.md#createpromptcategory) | **POST** /v2/prompts/categories/create | Create Prompt Category
*PromptsApi* | [**deletePrompt**](docs/PromptsApi.md#deleteprompt) | **DELETE** /v2/prompts/{prompt_id} | Delete Prompt
*PromptsApi* | [**deletePromptCategory**](docs/PromptsApi.md#deletepromptcategory) | **DELETE** /v2/prompts/categories/{cat_id} | Delete Prompt Category
*PromptsApi* | [**searchPromptCategories**](docs/PromptsApi.md#searchpromptcategories) | **POST** /v2/prompts/categories/search | Search Prompt Categories
*PromptsApi* | [**searchPrompts**](docs/PromptsApi.md#searchprompts) | **POST** /v2/prompts/search | Search Prompts
*PromptsApi* | [**updatePrompt**](docs/PromptsApi.md#updateprompt) | **PUT** /v2/prompts/{prompt_id} | Update Prompt
*PromptsApi* | [**updatePromptCategory**](docs/PromptsApi.md#updatepromptcategory) | **PUT** /v2/prompts/categories/{cat_id} | Update Prompt Category
*ReindexApi* | [**getReindexStatus**](docs/ReindexApi.md#getreindexstatus) | **GET** /v2/reindex/status | Get Reindex Status
*ReindexApi* | [**triggerReindex**](docs/ReindexApi.md#triggerreindex) | **POST** /v2/reindex/ | Trigger Reindex
*SERPApi* | [**searchClusterQuery**](docs/SERPApi.md#searchclusterquery) | **POST** /v2/serp/clusters/keywords | Search Cluster Query
*SERPApi* | [**serpClusterAddQueries**](docs/SERPApi.md#serpclusteraddqueries) | **POST** /v2/serp/clusters/{customer_id}/{campaign_id}/{group_id}/add_keywords | Serp Cluster Add Queries
*SERPApi* | [**serpClusterDeleteCampaign**](docs/SERPApi.md#serpclusterdeletecampaign) | **DELETE** /v2/serp/clusters/{customer_id}/{campaign_id} | Serp Cluster Delete Campaign
*SERPApi* | [**serpClusterDeleteCustomer**](docs/SERPApi.md#serpclusterdeletecustomer) | **DELETE** /v2/serp/clusters/{customer_id} | Serp Cluster Delete Customer
*SERPApi* | [**serpClusterDeleteGroup**](docs/SERPApi.md#serpclusterdeletegroup) | **DELETE** /v2/serp/clusters/{customer_id}/{campaign_id}/{group_id} | Serp Cluster Delete Group
*SERPApi* | [**serpClusterDeleteGroupQueries**](docs/SERPApi.md#serpclusterdeletegroupqueries) | **DELETE** /v2/serp/clusters/{customer_id}/{campaign_id}/{group_id}/delete_queries | Serp Cluster Delete Group Queries
*SERPApi* | [**serpClusterGetGraphNodes**](docs/SERPApi.md#serpclustergetgraphnodes) | **POST** /v2/serp/clusters/graph_nodes | Serp Cluster Get Graph Nodes
*SERPApi* | [**serpClusterGetMatchingGroupsToQuery**](docs/SERPApi.md#serpclustergetmatchinggroupstoquery) | **POST** /v2/serp/clusters/recommended_groups | Serp Cluster Get Matching Groups To Query
*SERPApi* | [**serpClusterGetRelatedKeywordsToQuery**](docs/SERPApi.md#serpclustergetrelatedkeywordstoquery) | **POST** /v2/serp/clusters/related_keywords | Serp Cluster Get Related Keywords To Query
*SERPApi* | [**serpClusterSplitToSubClusters**](docs/SERPApi.md#serpclustersplittosubclusters) | **POST** /v2/serp/clusters/split_sub_clusters | Serp Cluster Split To Sub Clusters
*SERPApi* | [**serpSearch**](docs/SERPApi.md#serpsearch) | **POST** /v2/serp/serp/search | Serp Search
*SERPApi* | [**serpVolumes**](docs/SERPApi.md#serpvolumes) | **POST** /v2/serp/serp/volumes | Serp Volumes
*SERPApi* | [**serpVolumesPingback**](docs/SERPApi.md#serpvolumespingback) | **GET** /v2/serp/serp/volumes/pingback/{id}/{tag} | Serp Volumes Pingback
*SchedulesApi* | [**createSchedules**](docs/SchedulesApi.md#createschedules) | **POST** /v2/schedules/create | Create Schedules
*SchedulesApi* | [**deleteSchedule**](docs/SchedulesApi.md#deleteschedule) | **DELETE** /v2/schedules/{schedule_id} | Delete Schedule
*SchedulesApi* | [**getSchedule**](docs/SchedulesApi.md#getschedule) | **GET** /v2/schedules/{schedule_id} | Get Schedule
*SchedulesApi* | [**getScheduleUrlDetails**](docs/SchedulesApi.md#getscheduleurldetails) | **GET** /v2/schedules/{schedule_id}/urls/{domain_id}/{url_id} | Get Schedule Url Details
*SchedulesApi* | [**getSchedules**](docs/SchedulesApi.md#getschedules) | **POST** /v2/schedules/ | Get Schedules
*SchedulesApi* | [**runSchedule**](docs/SchedulesApi.md#runschedule) | **POST** /v2/schedules/run/{schedule_id} | Run Schedule
*SchedulesApi* | [**searchScheduleUrls**](docs/SchedulesApi.md#searchscheduleurls) | **POST** /v2/schedules/urls/ | Search Schedule Urls
*SchedulesApi* | [**updateSchedule**](docs/SchedulesApi.md#updateschedule) | **PUT** /v2/schedules/{schedule_id} | Update Schedule
*SecretsApi* | [**createSecret**](docs/SecretsApi.md#createsecret) | **POST** /v2/secrets/create | Create Secret
*SecretsApi* | [**deleteSecret**](docs/SecretsApi.md#deletesecret) | **DELETE** /v2/secrets/{secret_id} | Delete Secret
*SecretsApi* | [**getSecret**](docs/SecretsApi.md#getsecret) | **GET** /v2/secrets/{secret_id} | Get Secret
*SecretsApi* | [**searchSecret**](docs/SecretsApi.md#searchsecret) | **POST** /v2/secrets/search | Search Secret
*SecretsApi* | [**updateSecret**](docs/SecretsApi.md#updatesecret) | **PUT** /v2/secrets/{secret_id} | Update Secret
*SemanticSearchApi* | [**getSimilarDocsByDocId**](docs/SemanticSearchApi.md#getsimilardocsbydocid) | **POST** /v2/similarities/document/live | Get Similar Docs By Doc Id
*SemanticSearchApi* | [**getSimilarDocsByQuery**](docs/SemanticSearchApi.md#getsimilardocsbyquery) | **POST** /v2/similarities/query/live | Get Similar Docs By Query
*SemanticSearchApi* | [**scheduleSimilarDocsByDocId**](docs/SemanticSearchApi.md#schedulesimilardocsbydocid) | **POST** /v2/similarities/document | Schedule Similar Docs By Doc Id
*SemanticSearchApi* | [**scheduleSimilarDocsByQuery**](docs/SemanticSearchApi.md#schedulesimilardocsbyquery) | **POST** /v2/similarities/query | Schedule Similar Docs By Query
*ShopifyApi* | [**customerDataRequest**](docs/ShopifyApi.md#customerdatarequest) | **POST** /v2/integrations/shopify/webhooks/customers/data_request | Customer Data Request
*ShopifyApi* | [**customerRedact**](docs/ShopifyApi.md#customerredact) | **POST** /v2/integrations/shopify/webhooks/customers/redact | Customer Redact
*ShopifyApi* | [**getShopify**](docs/ShopifyApi.md#getshopify) | **GET** /v2/integrations/shopify/ | Get Shopify
*ShopifyApi* | [**shopRedact**](docs/ShopifyApi.md#shopredact) | **POST** /v2/integrations/shopify/webhooks/shop/redact | Shop Redact
*ShopifyApi* | [**subscriptionCancel**](docs/ShopifyApi.md#subscriptioncancel) | **POST** /v2/integrations/shopify/webhooks/billing/subscription_cancel | Subscription Cancel
*ShopifyApi* | [**subscriptionUpdate**](docs/ShopifyApi.md#subscriptionupdate) | **POST** /v2/integrations/shopify/webhooks/billing/subscription_update | Subscription Update
*SlackApi* | [**getSlackChannels**](docs/SlackApi.md#getslackchannels) | **GET** /v2/integrations/slack/{slack_team_id}/channels | Get Slack Channels
*SlackApi* | [**getSlackWorkspaces**](docs/SlackApi.md#getslackworkspaces) | **GET** /v2/integrations/slack/ | Get Slack Workspaces
*TagsApi* | [**createTag**](docs/TagsApi.md#createtag) | **POST** /v2/tags/create | Create Tag
*TagsApi* | [**deleteTag**](docs/TagsApi.md#deletetag) | **DELETE** /v2/tags/{tag_id} | Delete Tag
*TagsApi* | [**searchTags**](docs/TagsApi.md#searchtags) | **POST** /v2/tags/search | Search Tags
*TagsApi* | [**updateTag**](docs/TagsApi.md#updatetag) | **PUT** /v2/tags/{tag_id} | Update Tag
*TrackingApi* | [**searchEvents**](docs/TrackingApi.md#searchevents) | **POST** /v2/tracking/events | Search Events
*TrackingApi* | [**searchLinks**](docs/TrackingApi.md#searchlinks) | **POST** /v2/tracking/links | Search Links
*TrackingApi* | [**searchSources**](docs/TrackingApi.md#searchsources) | **POST** /v2/tracking/sources | Search Sources
*TrackingApi* | [**trackClick**](docs/TrackingApi.md#trackclick) | **POST** /v2/tracking/clk | Track Click
*TrackingApi* | [**trackEvent**](docs/TrackingApi.md#trackevent) | **POST** /v2/tracking/evnt | Track Event
*TrackingApi* | [**trackLink**](docs/TrackingApi.md#tracklink) | **POST** /v2/tracking/lnk | Track Link
*WebAuthApi* | [**activateAccount**](docs/WebAuthApi.md#activateaccount) | **GET** /v2/auth/activate | Activate Account
*WebAuthApi* | [**getUser**](docs/WebAuthApi.md#getuser) | **GET** /v2/auth/me | Get User
*WebAuthApi* | [**passwordRecoveryPage**](docs/WebAuthApi.md#passwordrecoverypage) | **GET** /v2/auth/recover-password | Password Recovery Page
*WebAuthApi* | [**passwordRecoverySubmit**](docs/WebAuthApi.md#passwordrecoverysubmit) | **POST** /v2/auth/recover-password | Password Recovery Submit
*WebAuthApi* | [**registerPage**](docs/WebAuthApi.md#registerpage) | **GET** /v2/auth/register | Register Page
*WebAuthApi* | [**registerSubmit**](docs/WebAuthApi.md#registersubmit) | **POST** /v2/auth/register | Register Submit
*WebAuthApi* | [**resetPasswordPage**](docs/WebAuthApi.md#resetpasswordpage) | **GET** /v2/auth/reset-password | Reset Password Page
*WebAuthApi* | [**resetPasswordSubmit**](docs/WebAuthApi.md#resetpasswordsubmit) | **POST** /v2/auth/reset-password | Reset Password Submit
*WebAuthApi* | [**ssoLoginPage**](docs/WebAuthApi.md#ssologinpage) | **GET** /v2/auth/oauth/sso | Sso Login Page
*WebAuthApi* | [**ssoLoginSubmit**](docs/WebAuthApi.md#ssologinsubmit) | **POST** /v2/auth/oauth/sso | Sso Login Submit
*WordPressApi* | [**getWordpressPostCategories**](docs/WordPressApi.md#getwordpresspostcategories) | **GET** /v2/integrations/wordpress/{integration_id}/categories | Get Wordpress Post Categories
*WordPressApi* | [**getWordpressPostTags**](docs/WordPressApi.md#getwordpressposttags) | **GET** /v2/integrations/wordpress/{integration_id}/tags | Get Wordpress Post Tags
*WordPressApi* | [**getWordpressSites**](docs/WordPressApi.md#getwordpresssites) | **GET** /v2/integrations/wordpress/sites | Get Wordpress Sites
*WorkspacesApi* | [**addWorkspaceUser**](docs/WorkspacesApi.md#addworkspaceuser) | **POST** /v2/workspaces/{workspace_id}/add-member | Add Workspace User
*WorkspacesApi* | [**createWorkspace**](docs/WorkspacesApi.md#createworkspace) | **POST** /v2/workspaces/create | Create Workspace
*WorkspacesApi* | [**deleteWorkspace**](docs/WorkspacesApi.md#deleteworkspace) | **DELETE** /v2/workspaces/{workspace_id} | Delete Workspace
*WorkspacesApi* | [**deleteWorkspaceUser**](docs/WorkspacesApi.md#deleteworkspaceuser) | **DELETE** /v2/workspaces/{workspace_id}/{user_id} | Delete Workspace User
*WorkspacesApi* | [**getWorkspace**](docs/WorkspacesApi.md#getworkspace) | **POST** /v2/workspaces/{workspace_id} | Get Workspace
*WorkspacesApi* | [**searchMyWorkspaces**](docs/WorkspacesApi.md#searchmyworkspaces) | **POST** /v2/workspaces/me/my_workspaces | Search My Workspaces
*WorkspacesApi* | [**searchWorkspaceUsers**](docs/WorkspacesApi.md#searchworkspaceusers) | **POST** /v2/workspaces/{workspace_id}/users | Search Workspace Users
*WorkspacesApi* | [**updateWorkspace**](docs/WorkspacesApi.md#updateworkspace) | **PUT** /v2/workspaces/{workspace_id} | Update Workspace
*WorkspacesApi* | [**updateWorkspaceUser**](docs/WorkspacesApi.md#updateworkspaceuser) | **PUT** /v2/workspaces/{workspace_id}/{user_id} | Update Workspace User
*WorkspacesSSOApi* | [**createWorkspaceSsoSettings**](docs/WorkspacesSSOApi.md#createworkspacessosettings) | **POST** /v2/workspaces/{workspace_id}/sso | Create Workspace Sso Settings
*WorkspacesSSOApi* | [**deleteWorkspaceSsoSettings**](docs/WorkspacesSSOApi.md#deleteworkspacessosettings) | **DELETE** /v2/workspaces/{workspace_id}/sso/{provider} | Delete Workspace Sso Settings
*WorkspacesSSOApi* | [**getWorkspaceSsoSettings**](docs/WorkspacesSSOApi.md#getworkspacessosettings) | **GET** /v2/workspaces/{workspace_id}/sso/{provider} | Get Workspace Sso Settings
*WorkspacesSSOApi* | [**listWorkspaceSsoSettings**](docs/WorkspacesSSOApi.md#listworkspacessosettings) | **GET** /v2/workspaces/{workspace_id}/sso | List Workspace Sso Settings
*WorkspacesSSOApi* | [**updateWorkspaceSsoSettings**](docs/WorkspacesSSOApi.md#updateworkspacessosettings) | **PUT** /v2/workspaces/{workspace_id}/sso/{provider} | Update Workspace Sso Settings
*WorkspacesSSODomainVerificationApi* | [**createDomainVerification**](docs/WorkspacesSSODomainVerificationApi.md#createdomainverification) | **POST** /v2/workspaces/{workspace_id}/sso/domain-verification | Create Domain Verification
*WorkspacesSSODomainVerificationApi* | [**deleteDomainVerification**](docs/WorkspacesSSODomainVerificationApi.md#deletedomainverification) | **DELETE** /v2/workspaces/{workspace_id}/sso/domain-verification | Delete Domain Verification
*WorkspacesSSODomainVerificationApi* | [**listDomainVerifications**](docs/WorkspacesSSODomainVerificationApi.md#listdomainverifications) | **GET** /v2/workspaces/{workspace_id}/sso/domain-verification | List Domain Verifications
*WorkspacesSSODomainVerificationApi* | [**verifyDomain**](docs/WorkspacesSSODomainVerificationApi.md#verifydomain) | **POST** /v2/workspaces/{workspace_id}/sso/domain-verification/verify | Verify Domain


### Documentation For Models

 - [AddOnAddRequest](docs/AddOnAddRequest.md)
 - [AllFlowsSearchRequest](docs/AllFlowsSearchRequest.md)
 - [ApiKeyCreateRequest](docs/ApiKeyCreateRequest.md)
 - [ApiKeyResponse](docs/ApiKeyResponse.md)
 - [ApiKeySearchRequest](docs/ApiKeySearchRequest.md)
 - [ApiKeyUpdateRequest](docs/ApiKeyUpdateRequest.md)
 - [AppUrlInput](docs/AppUrlInput.md)
 - [AppUrlOutput](docs/AppUrlOutput.md)
 - [AspecRatio](docs/AspecRatio.md)
 - [BaseFoundationModel](docs/BaseFoundationModel.md)
 - [BillingProvider](docs/BillingProvider.md)
 - [BoolChar](docs/BoolChar.md)
 - [CategoryType](docs/CategoryType.md)
 - [ChartSessionDurationResponse](docs/ChartSessionDurationResponse.md)
 - [ChartsFeedbackRequest](docs/ChartsFeedbackRequest.md)
 - [ChatbotCreateRequest](docs/ChatbotCreateRequest.md)
 - [ChatbotResponse](docs/ChatbotResponse.md)
 - [ChatbotSearchRequest](docs/ChatbotSearchRequest.md)
 - [ChatbotStatus](docs/ChatbotStatus.md)
 - [ChatbotUpdateRequest](docs/ChatbotUpdateRequest.md)
 - [CheckoutCreateRequest](docs/CheckoutCreateRequest.md)
 - [CommunityImageGenerationsResponse](docs/CommunityImageGenerationsResponse.md)
 - [Completed](docs/Completed.md)
 - [CreditBalanceResponse](docs/CreditBalanceResponse.md)
 - [CreditDailyTransactionResponse](docs/CreditDailyTransactionResponse.md)
 - [CreditDailyTransactionSearchRequest](docs/CreditDailyTransactionSearchRequest.md)
 - [CreditTransactionResponse](docs/CreditTransactionResponse.md)
 - [CreditTransactionSearchRequest](docs/CreditTransactionSearchRequest.md)
 - [CustomerDataRequestPayload](docs/CustomerDataRequestPayload.md)
 - [CustomerRedactPayload](docs/CustomerRedactPayload.md)
 - [Data](docs/Data.md)
 - [DeleteNodeRequest](docs/DeleteNodeRequest.md)
 - [DocumentCategoryCreateRequest](docs/DocumentCategoryCreateRequest.md)
 - [DocumentCategoryResponse](docs/DocumentCategoryResponse.md)
 - [DocumentCategorySearchRequest](docs/DocumentCategorySearchRequest.md)
 - [DocumentCategoryUpdateRequest](docs/DocumentCategoryUpdateRequest.md)
 - [DocumentContent](docs/DocumentContent.md)
 - [DocumentContentResponse](docs/DocumentContentResponse.md)
 - [DocumentResponse](docs/DocumentResponse.md)
 - [DocumentSearchRequest](docs/DocumentSearchRequest.md)
 - [DocumentSimilarityRequest](docs/DocumentSimilarityRequest.md)
 - [DocumentSimilarityTaskRequest](docs/DocumentSimilarityTaskRequest.md)
 - [DocumentStatus](docs/DocumentStatus.md)
 - [DocumentType](docs/DocumentType.md)
 - [DocumentUpdateRequest](docs/DocumentUpdateRequest.md)
 - [DriverSuccessResponse](docs/DriverSuccessResponse.md)
 - [DriverType](docs/DriverType.md)
 - [FTStatus](docs/FTStatus.md)
 - [FTType](docs/FTType.md)
 - [FailedFaqItem](docs/FailedFaqItem.md)
 - [FaqCreateRequest](docs/FaqCreateRequest.md)
 - [FaqImportResponse](docs/FaqImportResponse.md)
 - [FaqResponse](docs/FaqResponse.md)
 - [FaqSearchRequest](docs/FaqSearchRequest.md)
 - [FaqStatus](docs/FaqStatus.md)
 - [FaqType](docs/FaqType.md)
 - [FaqUpdateRequest](docs/FaqUpdateRequest.md)
 - [FeatureResponse](docs/FeatureResponse.md)
 - [FeedbackChartResponse](docs/FeedbackChartResponse.md)
 - [FileUploadResponse](docs/FileUploadResponse.md)
 - [FlowAssistantAIModel](docs/FlowAssistantAIModel.md)
 - [FlowAssistantAddComponentMetadata](docs/FlowAssistantAddComponentMetadata.md)
 - [FlowAssistantAddConnectionMetadata](docs/FlowAssistantAddConnectionMetadata.md)
 - [FlowAssistantApplyRejectChangesRequest](docs/FlowAssistantApplyRejectChangesRequest.md)
 - [FlowAssistantCreateBlankFlowMetadata](docs/FlowAssistantCreateBlankFlowMetadata.md)
 - [FlowAssistantDeleteComponentMetadata](docs/FlowAssistantDeleteComponentMetadata.md)
 - [FlowAssistantDeleteConnectionMetadata](docs/FlowAssistantDeleteConnectionMetadata.md)
 - [FlowAssistantInvokeRequest](docs/FlowAssistantInvokeRequest.md)
 - [FlowAssistantSessionCreateRequest](docs/FlowAssistantSessionCreateRequest.md)
 - [FlowAssistantUpdateComponentMetadata](docs/FlowAssistantUpdateComponentMetadata.md)
 - [FlowBranch](docs/FlowBranch.md)
 - [FlowCategoryCreateRequest](docs/FlowCategoryCreateRequest.md)
 - [FlowCategoryResponse](docs/FlowCategoryResponse.md)
 - [FlowCategorySearchRequest](docs/FlowCategorySearchRequest.md)
 - [FlowCommitRequest](docs/FlowCommitRequest.md)
 - [FlowCommitResponse](docs/FlowCommitResponse.md)
 - [FlowConfig](docs/FlowConfig.md)
 - [FlowCreate](docs/FlowCreate.md)
 - [FlowCronCreateRequest](docs/FlowCronCreateRequest.md)
 - [FlowCronResponse](docs/FlowCronResponse.md)
 - [FlowCronSearchRequest](docs/FlowCronSearchRequest.md)
 - [FlowCronStatus](docs/FlowCronStatus.md)
 - [FlowCronUpdateRequest](docs/FlowCronUpdateRequest.md)
 - [FlowDetailResponse](docs/FlowDetailResponse.md)
 - [FlowEventActionType](docs/FlowEventActionType.md)
 - [FlowHuntProductSlug](docs/FlowHuntProductSlug.md)
 - [FlowInvokeRequest](docs/FlowInvokeRequest.md)
 - [FlowMessageFeedbackRequest](docs/FlowMessageFeedbackRequest.md)
 - [FlowMessageFeedbackResponse](docs/FlowMessageFeedbackResponse.md)
 - [FlowResponse](docs/FlowResponse.md)
 - [FlowSearchRequest](docs/FlowSearchRequest.md)
 - [FlowSessionAttachmentResponse](docs/FlowSessionAttachmentResponse.md)
 - [FlowSessionCreateFromFlowRequest](docs/FlowSessionCreateFromFlowRequest.md)
 - [FlowSessionCreateRequest](docs/FlowSessionCreateRequest.md)
 - [FlowSessionEvent](docs/FlowSessionEvent.md)
 - [FlowSessionInvocationResponse](docs/FlowSessionInvocationResponse.md)
 - [FlowSessionInvokeRequest](docs/FlowSessionInvokeRequest.md)
 - [FlowSessionLoadingMetadata](docs/FlowSessionLoadingMetadata.md)
 - [FlowSessionMessageFeedbackMetadata](docs/FlowSessionMessageFeedbackMetadata.md)
 - [FlowSessionMessageMetadata](docs/FlowSessionMessageMetadata.md)
 - [FlowSessionResponse](docs/FlowSessionResponse.md)
 - [FlowSessionTaskResponseMetadata](docs/FlowSessionTaskResponseMetadata.md)
 - [FlowSessionToolCallMetadata](docs/FlowSessionToolCallMetadata.md)
 - [FlowSessionViewResponse](docs/FlowSessionViewResponse.md)
 - [FlowSessionViewSearchRequest](docs/FlowSessionViewSearchRequest.md)
 - [FlowSessionViewUpdateRequest](docs/FlowSessionViewUpdateRequest.md)
 - [FlowType](docs/FlowType.md)
 - [FlowUpdate](docs/FlowUpdate.md)
 - [FlowVersionHistoryResponse](docs/FlowVersionHistoryResponse.md)
 - [GeneralMCPSubserverCapabilitiesResponse](docs/GeneralMCPSubserverCapabilitiesResponse.md)
 - [GeneralMCPSubserverResponse](docs/GeneralMCPSubserverResponse.md)
 - [GetNodeRequest](docs/GetNodeRequest.md)
 - [GoogleAdsActionType](docs/GoogleAdsActionType.md)
 - [GoogleAdsAnalyzeKeywordsRequest](docs/GoogleAdsAnalyzeKeywordsRequest.md)
 - [GoogleAdsCampaignResponse](docs/GoogleAdsCampaignResponse.md)
 - [GoogleAdsCampaignStatus](docs/GoogleAdsCampaignStatus.md)
 - [GoogleAdsCampaignUpdateRequest](docs/GoogleAdsCampaignUpdateRequest.md)
 - [GoogleAdsCampaignsResponse](docs/GoogleAdsCampaignsResponse.md)
 - [GoogleAdsCampaignsSearchRequest](docs/GoogleAdsCampaignsSearchRequest.md)
 - [GoogleAdsCustomerResponse](docs/GoogleAdsCustomerResponse.md)
 - [GoogleAdsCustomerUpdateRequest](docs/GoogleAdsCustomerUpdateRequest.md)
 - [GoogleAdsCustomersResponse](docs/GoogleAdsCustomersResponse.md)
 - [GoogleAdsCustomersSearchRequest](docs/GoogleAdsCustomersSearchRequest.md)
 - [GoogleAdsGroupResponse](docs/GoogleAdsGroupResponse.md)
 - [GoogleAdsGroupStatus](docs/GoogleAdsGroupStatus.md)
 - [GoogleAdsGroupUpdateRequest](docs/GoogleAdsGroupUpdateRequest.md)
 - [GoogleAdsGroupsResponse](docs/GoogleAdsGroupsResponse.md)
 - [GoogleAdsGroupsSearchRequest](docs/GoogleAdsGroupsSearchRequest.md)
 - [GoogleAdsKeywordAddRequest](docs/GoogleAdsKeywordAddRequest.md)
 - [GoogleAdsKeywordRecommendation](docs/GoogleAdsKeywordRecommendation.md)
 - [GoogleAdsKeywordRemoveRequest](docs/GoogleAdsKeywordRemoveRequest.md)
 - [GoogleAdsMatchType](docs/GoogleAdsMatchType.md)
 - [GoogleAdsRecommendation](docs/GoogleAdsRecommendation.md)
 - [GoogleAdsRecommendationConfidence](docs/GoogleAdsRecommendationConfidence.md)
 - [GoogleAdsRecommendationStatus](docs/GoogleAdsRecommendationStatus.md)
 - [GoogleAdsRecommendationType](docs/GoogleAdsRecommendationType.md)
 - [GoogleAdsRecommendationsRequest](docs/GoogleAdsRecommendationsRequest.md)
 - [GoogleCalendarResponse](docs/GoogleCalendarResponse.md)
 - [GoogleCalendarsResponse](docs/GoogleCalendarsResponse.md)
 - [GooglePickerTokenResponse](docs/GooglePickerTokenResponse.md)
 - [GoogleSheetResponse](docs/GoogleSheetResponse.md)
 - [GoogleSheetsResponse](docs/GoogleSheetsResponse.md)
 - [HTTPValidationError](docs/HTTPValidationError.md)
 - [Health](docs/Health.md)
 - [HubSpotActorIdResponse](docs/HubSpotActorIdResponse.md)
 - [HubSpotActorsResponse](docs/HubSpotActorsResponse.md)
 - [HumanAgentSender](docs/HumanAgentSender.md)
 - [ImageConvertRequest](docs/ImageConvertRequest.md)
 - [ImageFTCreateRequest](docs/ImageFTCreateRequest.md)
 - [ImageFTResponse](docs/ImageFTResponse.md)
 - [ImageFTSearchRequest](docs/ImageFTSearchRequest.md)
 - [ImageFTUpdateRequest](docs/ImageFTUpdateRequest.md)
 - [ImageInferenceRequest](docs/ImageInferenceRequest.md)
 - [ImageInferenceResponse](docs/ImageInferenceResponse.md)
 - [ImageInferenceResultResponse](docs/ImageInferenceResultResponse.md)
 - [ImageInferenceScheduleResponse](docs/ImageInferenceScheduleResponse.md)
 - [ImageInferenceScrollResponse](docs/ImageInferenceScrollResponse.md)
 - [ImageOptimizeRequest](docs/ImageOptimizeRequest.md)
 - [ImagePromptGenerationRequest](docs/ImagePromptGenerationRequest.md)
 - [ImagePromptResponse](docs/ImagePromptResponse.md)
 - [InferenceFileType](docs/InferenceFileType.md)
 - [InferenceHistorySearchRequest](docs/InferenceHistorySearchRequest.md)
 - [InstagramProfileInformationResponse](docs/InstagramProfileInformationResponse.md)
 - [IntegrationCategory](docs/IntegrationCategory.md)
 - [IntegrationDetailResponse](docs/IntegrationDetailResponse.md)
 - [IntegrationFlowResponse](docs/IntegrationFlowResponse.md)
 - [IntegrationResponse](docs/IntegrationResponse.md)
 - [IntegrationSearchRequest](docs/IntegrationSearchRequest.md)
 - [IntegrationSlug](docs/IntegrationSlug.md)
 - [LangfuseRequest](docs/LangfuseRequest.md)
 - [LogEntryLevel](docs/LogEntryLevel.md)
 - [LogEntryType](docs/LogEntryType.md)
 - [LogResponse](docs/LogResponse.md)
 - [LogsSearchRequest](docs/LogsSearchRequest.md)
 - [MCPCapabilityBinding](docs/MCPCapabilityBinding.md)
 - [MCPServerCreateRequest](docs/MCPServerCreateRequest.md)
 - [MCPServerResponse](docs/MCPServerResponse.md)
 - [MCPServerSearchRequest](docs/MCPServerSearchRequest.md)
 - [MCPSubServerBinding](docs/MCPSubServerBinding.md)
 - [MemoryDocumentProcessRequest](docs/MemoryDocumentProcessRequest.md)
 - [MemoryDocumentUploadResponse](docs/MemoryDocumentUploadResponse.md)
 - [MemoryMessageResponse](docs/MemoryMessageResponse.md)
 - [MemoryNodeDetailResponse](docs/MemoryNodeDetailResponse.md)
 - [MemoryNodeNameSearchRequest](docs/MemoryNodeNameSearchRequest.md)
 - [MemoryNodePathSearchRequest](docs/MemoryNodePathSearchRequest.md)
 - [MemoryNodeResponse](docs/MemoryNodeResponse.md)
 - [MemorySearchRequest](docs/MemorySearchRequest.md)
 - [MemorySearchResponse](docs/MemorySearchResponse.md)
 - [MessageFeedback](docs/MessageFeedback.md)
 - [MessageType](docs/MessageType.md)
 - [Metadata](docs/Metadata.md)
 - [MicrosoftPowerBiDatasetResponse](docs/MicrosoftPowerBiDatasetResponse.md)
 - [MicrosoftPowerBiDatasetsResponse](docs/MicrosoftPowerBiDatasetsResponse.md)
 - [MicrosoftPowerBiPushDatasetResponse](docs/MicrosoftPowerBiPushDatasetResponse.md)
 - [MicrosoftPowerBiTableResponse](docs/MicrosoftPowerBiTableResponse.md)
 - [MicrosoftPowerBiTableValidateResponse](docs/MicrosoftPowerBiTableValidateResponse.md)
 - [MicrosoftPowerBiTablesResponse](docs/MicrosoftPowerBiTablesResponse.md)
 - [MicrosoftPowerBiWorkspaceResponse](docs/MicrosoftPowerBiWorkspaceResponse.md)
 - [MicrosoftPowerBiWorkspacesResponse](docs/MicrosoftPowerBiWorkspacesResponse.md)
 - [NodeDetailRequest](docs/NodeDetailRequest.md)
 - [NodeType](docs/NodeType.md)
 - [NodeUpdateRequest](docs/NodeUpdateRequest.md)
 - [ObservabilityDriverResponse](docs/ObservabilityDriverResponse.md)
 - [Pagination](docs/Pagination.md)
 - [PerDayFeedback](docs/PerDayFeedback.md)
 - [PerDaySessionDurationResponse](docs/PerDaySessionDurationResponse.md)
 - [PhotoAIEffectResponse](docs/PhotoAIEffectResponse.md)
 - [PhotoAIStyleResponse](docs/PhotoAIStyleResponse.md)
 - [PhotoAITemplateResponse](docs/PhotoAITemplateResponse.md)
 - [PlanListItemResponse](docs/PlanListItemResponse.md)
 - [PlanResponse](docs/PlanResponse.md)
 - [PointerType](docs/PointerType.md)
 - [PowerBiDatasetRequest](docs/PowerBiDatasetRequest.md)
 - [PowerBiPushDatasetRequest](docs/PowerBiPushDatasetRequest.md)
 - [PowerBiRequest](docs/PowerBiRequest.md)
 - [PowerBiTableRequest](docs/PowerBiTableRequest.md)
 - [PromptCategoryCreateRequest](docs/PromptCategoryCreateRequest.md)
 - [PromptCategoryResponse](docs/PromptCategoryResponse.md)
 - [PromptCategorySearchRequest](docs/PromptCategorySearchRequest.md)
 - [PromptCategoryUpdateRequest](docs/PromptCategoryUpdateRequest.md)
 - [PromptCreateRequest](docs/PromptCreateRequest.md)
 - [PromptResponse](docs/PromptResponse.md)
 - [PromptSearchRequest](docs/PromptSearchRequest.md)
 - [PromptUpdateRequest](docs/PromptUpdateRequest.md)
 - [QuerySimilarityRequest](docs/QuerySimilarityRequest.md)
 - [QuerySimilarityTaskRequest](docs/QuerySimilarityTaskRequest.md)
 - [ReindexDataSource](docs/ReindexDataSource.md)
 - [ReindexProgress](docs/ReindexProgress.md)
 - [ReindexRequest](docs/ReindexRequest.md)
 - [ReindexScope](docs/ReindexScope.md)
 - [ReindexStartResponse](docs/ReindexStartResponse.md)
 - [ReindexStatus](docs/ReindexStatus.md)
 - [ReindexStatusResponse](docs/ReindexStatusResponse.md)
 - [Role](docs/Role.md)
 - [SamlLoginMethod](docs/SamlLoginMethod.md)
 - [ScheduleCreateRequest](docs/ScheduleCreateRequest.md)
 - [ScheduleFrequency](docs/ScheduleFrequency.md)
 - [ScheduleResponse](docs/ScheduleResponse.md)
 - [ScheduleSearchRequest](docs/ScheduleSearchRequest.md)
 - [ScheduleStatus](docs/ScheduleStatus.md)
 - [ScheduleType](docs/ScheduleType.md)
 - [ScheduleUpdateRequest](docs/ScheduleUpdateRequest.md)
 - [ScheduleUrlDetailResponse](docs/ScheduleUrlDetailResponse.md)
 - [ScheduleUrlResponse](docs/ScheduleUrlResponse.md)
 - [ScheduleUrlSearchRequest](docs/ScheduleUrlSearchRequest.md)
 - [ScreenshotRequest](docs/ScreenshotRequest.md)
 - [ScreenshotResponse](docs/ScreenshotResponse.md)
 - [SearchType](docs/SearchType.md)
 - [SecretCreateRequest](docs/SecretCreateRequest.md)
 - [SecretResponse](docs/SecretResponse.md)
 - [SecretSearchRequest](docs/SecretSearchRequest.md)
 - [SecretUpdateRequest](docs/SecretUpdateRequest.md)
 - [SerpClusterAddQueryRequest](docs/SerpClusterAddQueryRequest.md)
 - [SerpClusterAddQueryRequests](docs/SerpClusterAddQueryRequests.md)
 - [SerpClusterBestGroupsRequest](docs/SerpClusterBestGroupsRequest.md)
 - [SerpClusterGroupIntersectionsRequest](docs/SerpClusterGroupIntersectionsRequest.md)
 - [SerpClusterGroupSearchRequest](docs/SerpClusterGroupSearchRequest.md)
 - [SerpClusterGroupSubClustersRequest](docs/SerpClusterGroupSubClustersRequest.md)
 - [SerpClusterKeywordIntersectionsRequest](docs/SerpClusterKeywordIntersectionsRequest.md)
 - [SerpClusterKeywordResponse](docs/SerpClusterKeywordResponse.md)
 - [SerpGroupIntersection](docs/SerpGroupIntersection.md)
 - [SerpKeyword](docs/SerpKeyword.md)
 - [SerpKeywordRelation](docs/SerpKeywordRelation.md)
 - [SerpQueryRequest](docs/SerpQueryRequest.md)
 - [SerpSearchEngineType](docs/SerpSearchEngineType.md)
 - [SerpSearchRequest](docs/SerpSearchRequest.md)
 - [SerpSearchRequests](docs/SerpSearchRequests.md)
 - [SerpSubclusterKeywordsResponse](docs/SerpSubclusterKeywordsResponse.md)
 - [SerpVolumeRequest](docs/SerpVolumeRequest.md)
 - [ShopRedactPayload](docs/ShopRedactPayload.md)
 - [ShopifyIntegrationResponse](docs/ShopifyIntegrationResponse.md)
 - [ShopifySubscriptionConfirmResponse](docs/ShopifySubscriptionConfirmResponse.md)
 - [SlackChannelResponse](docs/SlackChannelResponse.md)
 - [SlackWorkspaceResponse](docs/SlackWorkspaceResponse.md)
 - [SortDirection](docs/SortDirection.md)
 - [Source](docs/Source.md)
 - [SubscriptionPlan](docs/SubscriptionPlan.md)
 - [SystemMessageMetadata](docs/SystemMessageMetadata.md)
 - [TagCreateRequest](docs/TagCreateRequest.md)
 - [TagResponse](docs/TagResponse.md)
 - [TagSearchRequest](docs/TagSearchRequest.md)
 - [TagUpdateRequest](docs/TagUpdateRequest.md)
 - [TaskResponse](docs/TaskResponse.md)
 - [TaskStatus](docs/TaskStatus.md)
 - [ToolCallFeedbackResponse](docs/ToolCallFeedbackResponse.md)
 - [ToolFeedback](docs/ToolFeedback.md)
 - [TotalFeedback](docs/TotalFeedback.md)
 - [TrackingClickIdNames](docs/TrackingClickIdNames.md)
 - [TrackingEventCreateRequest](docs/TrackingEventCreateRequest.md)
 - [TrackingEventCreateRequests](docs/TrackingEventCreateRequests.md)
 - [TrackingEventData](docs/TrackingEventData.md)
 - [TrackingEventResponse](docs/TrackingEventResponse.md)
 - [TrackingEventSearchRequest](docs/TrackingEventSearchRequest.md)
 - [TrackingEventsResponse](docs/TrackingEventsResponse.md)
 - [TrackingLinkCreateRequest](docs/TrackingLinkCreateRequest.md)
 - [TrackingLinkResponse](docs/TrackingLinkResponse.md)
 - [TrackingLinkSearchRequest](docs/TrackingLinkSearchRequest.md)
 - [TrackingLinksCreateRequest](docs/TrackingLinksCreateRequest.md)
 - [TrackingLinksResponse](docs/TrackingLinksResponse.md)
 - [TrackingSourceCreateRequest](docs/TrackingSourceCreateRequest.md)
 - [TrackingSourceResponse](docs/TrackingSourceResponse.md)
 - [TrackingSourceSearchRequest](docs/TrackingSourceSearchRequest.md)
 - [TrackingSourceTypes](docs/TrackingSourceTypes.md)
 - [TrackingSourcesResponse](docs/TrackingSourcesResponse.md)
 - [TransactionType](docs/TransactionType.md)
 - [TranscriptTaskRequest](docs/TranscriptTaskRequest.md)
 - [TriggerResponse](docs/TriggerResponse.md)
 - [TriggerType](docs/TriggerType.md)
 - [UpdateUserSettingsRequest](docs/UpdateUserSettingsRequest.md)
 - [UrlScreenshotResponse](docs/UrlScreenshotResponse.md)
 - [UserDocumentStatus](docs/UserDocumentStatus.md)
 - [UserPlanResponse](docs/UserPlanResponse.md)
 - [UserResponse](docs/UserResponse.md)
 - [UserSettingsResponse](docs/UserSettingsResponse.md)
 - [ValidationError](docs/ValidationError.md)
 - [ValidationErrorLocInner](docs/ValidationErrorLocInner.md)
 - [VectorDocumentResponse](docs/VectorDocumentResponse.md)
 - [VectorDocumentType](docs/VectorDocumentType.md)
 - [VectorDocumentsTaskResponse](docs/VectorDocumentsTaskResponse.md)
 - [WordPressCategoryResponse](docs/WordPressCategoryResponse.md)
 - [WordPressSiteResponse](docs/WordPressSiteResponse.md)
 - [WordPressTagsResponse](docs/WordPressTagsResponse.md)
 - [WorkspaceCreateRequest](docs/WorkspaceCreateRequest.md)
 - [WorkspaceResponse](docs/WorkspaceResponse.md)
 - [WorkspaceRole](docs/WorkspaceRole.md)
 - [WorkspaceSSOCreateRequest](docs/WorkspaceSSOCreateRequest.md)
 - [WorkspaceSSODomainVerificationCreateRequest](docs/WorkspaceSSODomainVerificationCreateRequest.md)
 - [WorkspaceSSODomainVerificationResponse](docs/WorkspaceSSODomainVerificationResponse.md)
 - [WorkspaceSSOListResponse](docs/WorkspaceSSOListResponse.md)
 - [WorkspaceSSOResponse](docs/WorkspaceSSOResponse.md)
 - [WorkspaceSSOUpdateRequest](docs/WorkspaceSSOUpdateRequest.md)
 - [WorkspaceSearchRequest](docs/WorkspaceSearchRequest.md)
 - [WorkspaceUpdateRequest](docs/WorkspaceUpdateRequest.md)
 - [WorkspaceUserCreateRequest](docs/WorkspaceUserCreateRequest.md)
 - [WorkspaceUserResponse](docs/WorkspaceUserResponse.md)
 - [WorkspaceUserUpdateRequest](docs/WorkspaceUserUpdateRequest.md)
 - [WorkspaceUsersSearchRequest](docs/WorkspaceUsersSearchRequest.md)
 - [YoutubeContent](docs/YoutubeContent.md)
 - [YoutubeTranscriptRequest](docs/YoutubeTranscriptRequest.md)
 - [YoutubeTranscriptResponse](docs/YoutubeTranscriptResponse.md)


<a id="documentation-for-authorization"></a>
## Documentation For Authorization


Authentication schemes defined for the API:
<a id="APIKeyHeader"></a>
### APIKeyHeader

- **Type**: API key
- **API key parameter name**: Api-Key
- **Location**: HTTP header

<a id="HTTPBearer"></a>
### HTTPBearer

- **Type**: Bearer authentication

<a id="sudo_api_key_header"></a>
### sudo_api_key_header

- **Type**: API key
- **API key parameter name**: Sudo-Api-Key
- **Location**: HTTP header

