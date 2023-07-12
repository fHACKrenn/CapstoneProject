# CapstoneProject
This repository contains Capstone Project as final project of Hybrid Cloud and AI intership at Infinite Learning.
The application made is a chatbot named Vainglory Assistant to help maintain website at [here](https://vainglorydraft.fhackrenn.repl.co/). The purpose is to ease people if they have questions or technical issues regarding Vainglory using Watson Assistant service and Watson Discovery as its search skill.

The website works as a draft simulator for Vainglory. Original repository of the website can be checked at [Vainglory Draft](https://github.com/fHACKrenn/VaingloryDraft). Installation of the website along with error handling and commits/updates is maintained there.

## Project Description

### Developer Profile
| Name                  |<span style="font-weight:normal">Fachrendy Zulfikar Abdillah</span>|
|:----------------------|:------------------------------------------------------------------|
| **University**        | Sepuluh Nopember Institute of Technology                          |
| **Personal Mentor**   | Agistira Lamunde                                                  |


### Project Details
| Project Category      |<span style="font-weight:normal">Artificial Intelligence</span>    |
|:----------------------|:------------------------------------------------------------------|
| **Project Name**      | Integration of IBM Watson Assistant and Watson Discovery in Enhancing Information System Functions on Websites through Virtual Assistants                                                 |
| **Pattern**           | [Enhance customer helpdesks with Smart Document Understanding using the Watson Assistant search skill](https://developer.ibm.com/patterns/enhance-customer-helpdesk-with-smart-document-understanding-using-search-skill/ "Project's Pattern")                      |
| **IBM Features**      | Watson Assistant, Watson Discovery                                |
| **Project Site**      | https://vainglorydraft.fhackrenn.repl.co/                                |

## Documentary of Watson Assistant
### Code
Watson Assistant and Watson Discovery don't do much coding. [VaingloryAssistant-dialog.json](https://github.com/fHACKrenn/CapstoneProject/blob/master/VaingloryAssistant-dialog.json "Dialog Structure") is a json file that contains dialog structure of Watson Assistant.

To integrate Watson Assistant to a website. Watson Assistant provide an embed code to use the assistant on a website. The embed code has to be put inside html file.

The embed structure of integrating watson assistant as follows:
```html
<script>
  window.watsonAssistantChatOptions = {
    integrationID: INTEGRATION_ID, // The ID of this integration.
    region: REGION_HOST, // The region your integration is hosted in.
    serviceInstanceID: SERVICE_ID, // The ID of your service instance.
    onLoad: function(instance) { instance.render(); }
  };
  setTimeout(function(){
    const t=document.createElement('script');
    t.src="https://web-chat.global.assistant.watson.appdomain.cloud/versions/" + (window.watsonAssistantChatOptions.clientVersion || 'latest') + "/WatsonAssistantChatEntry.js";
    document.head.appendChild(t);
  });
</script>
```

### Dialog Intents
Intents list of watson assistant
![Dialog Intents](https://github.com/fHACKrenn/CapstoneProject/blob/master/src/images/dialogIntents.png?raw=true)

### Dialog Entities
Entities list of watson assistant
![Dialog Entities](https://github.com/fHACKrenn/CapstoneProject/blob/master/src/images/dialogEntities.png?raw=true)

### Dialog Structure
Dialog structure of watson assistant
![Dialog Structure](https://github.com/fHACKrenn/CapstoneProject/blob/master/src/images/dialogStructure.png?raw=true)

### Dialog Structure of Discovery Search Skill
Dialog structure of watson assistant that connects to Watson Discovery for search skill
![Dialog Structure Discover](https://github.com/fHACKrenn/CapstoneProject/blob/master/src/images/dialogStructureDiscovery.png?raw=true)

### Discovery Web Crawl
Usage of Watson Discovery. In this case, watson discovery use website as data source
![Discovery Web Crawl](https://github.com/fHACKrenn/CapstoneProject/blob/master/src/images/discoveryWebCrawl.png?raw=true)

### Assistant Home Screen
![Assistant Home Screen](https://github.com/fHACKrenn/CapstoneProject/blob/master/src/images/assistantHomeScreen.png?raw=true)

### Assistant Dialog Skill
![Assistant Dialog Skill](https://github.com/fHACKrenn/CapstoneProject/blob/master/src/images/assistantDialogSkill.png?raw=true)

### Assistant Search Skill
![Assistant Search Skill](https://github.com/fHACKrenn/CapstoneProject/blob/master/src/images/assistantSearchSkill.png?raw=true)
