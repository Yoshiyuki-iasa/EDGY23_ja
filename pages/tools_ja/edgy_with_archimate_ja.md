---
title_en: "EDGY with ArchiMate(tm)"
title_ja: "EDGYとArchiMate"
keywords: 
source_url: https://enterprise.design/wiki/EDGY:ArchiMate
source_last_modified: 14 July 2023, at 14:08
folder: pages/tools_ja
summary:
tags: 
  - 
---
# EDGY with ArchiMate®
Author credits: Milan Guenther, Marc Lankhorst, Jean-Baptiste Sarrodie. Thank you to Annika Klyver, Joost Lommers, Robert Pike and Wolfgang Goebl. ArchiMate® is a registered trademark of The Open Group®.

This mapping links EDGY Enterprise Elements to corresponding ArchiMate® elements. More specifically, EDGY elements can be represented as specialisations of corresponding ArchiMate elements. For more information on this mechanism, see the specialisation of concepts chapter in the official documentation.

## Using this mapping
This mapping has been designed based on the idea that EDGY specifically, and Enterprise Design in general, will be used to frame the strategic context of an initiative. Therefore this proposed mapping to ArchiMate® purposefully focuses on motivation elements and the strategy layer, while core elements can then be used to work on other layers not directly covered by EDGY. There are alternative mappings possible depending on the context of use.

Through the specialisation mechanism of ArchiMate® 3.2, any capable tool or environment can be used to model enterprises with EDGY elements. This mapping is designed with two main use cases in mind:

1. Using ArchiMate® to create an enterprise model with EDGY only: to take advantage of a repository based modelling tool rather than a purely graphical diagram editor or whiteboard, ArchiMate® elements and relations provide an invisible backbone underlying the model. Every EDGY element or relation will correspond to an ArchiMate® element or relation, but the depiction of each map (view) follows only the EDGY diagram depiction.
2. Using EDGY in combination with ArchiMate®: in this scenario both languages are used together as part of the same model. EDGY is used to create maps representing identity and experience facets. A high level architecture modelled using EDGY can then be detailed and guided into implementation using more specific ArchiMate® viewpoints, taking advantage of the more rich and rigorous language features.

## Base Elements
EDGY's base elements build a common vocabulary across all facets. They conceptually correspond to types as used in ArchiMate® (active and passive structures, behaviour and motivation). But unlike these categories, they are used to model the interplay of enterprise elements not specifically covered by the facet and intersection elements, so they map to concrete ArchiMate® elements.

![EDGY Base Elements ArchiMate mapping.png]

|EDGY Element|ArchiMate® Element|Observations|
|---|---|---|
|people|Stakeholder|EDGY is people-centric: people refers to any person or group, including legal entities. In ArchiMate®, people correspond to stakeholders that represent their interest in the effect of the architecture.|
|outcome|Outcome|Both languages use an outcome element to model an end result.|
|activity|Value Stream|In EDGY activities are used to model anything going on. The closest universal ArchiMate® concept is a value stream.|
|object|Resource|EDGY uses object as a universal base element for any structure or thing relevant to the enterprise. The closest ArchiMate® equivalent is a resource owned or controlled by an individual or an organisation.|

## Facet and Intersection Elements
In EDGY, the following elements are directly tied to the questions and topics raised within the realm of the corresponding enterprise design facets and their direct overlaps, with a different scope compared to layers and categories in ArchiMate®. This mapping follows the idea of framing initiatives strategically using EDGY, aligning with strategy, motivation and one business element in ArchiMate. This mapping prefers such a use case over linguistically more direct mappings such as EDGY process to ArchiMate® process, which is a suitable alternative if it matches better in a specific context of use.

![EDGY Facet Intersection Elements ArchiMate mapping.png]

|EDGY Element|ArchiMate® Element|Observations|
|---|---|---|
|purpose|Goal|An enterprise purpose is a kind of goal the enterprise pursues, therefore it maps to the goal element in ArchiMate®.|
|story|Course of Action|In EDGY story contextualises and explains the enterprise ambitions, which corresponds to a type of course of action in ArchiMate®.|
|content|Resource|There is no direct equivalent to content in ArchiMate®, but it can be represented as a type of resource.|
|organisation|Resource|Organisation in EDGY refers to any group of people working together, which can be best represented as a kind of (human) resource in ArchiMate®.|
|capability|Capability|Both EDGY and ArchiMate® share similar element definitions and use for capability.|
|process|Value Stream|A process in EDGY is closer to the value stream element in ArchiMate® than to the business process element, used for more detailed process descriptions and scenarios.|
|asset|Resource|EDGY uses a single element for various types of assets that are further distinguished in ArchiMate®. The most universal equivalent is resource.|
|product|Product|Both languages feature a versatile element to designate products as the result of an enterprise's activity. This is the only Core element featured in this mapping because of a large conceptual overlap.|
|task|Goal|A personal motivation of a customer or other people as defined in EDGY corresponds to a type of goal someone seeks to complete in ArchiMate®.|
|journey|Value Stream|ArchiMate® doesn't have a journey element, so a journey according to EDGY's definition is best represented as a type of value stream connected to a specific stakeholder.|
|channel|Resource|in EDGY, channels are means of interaction or communication such as media or physical environments. In ArchiMate® this is best represented as a type of resource used by the enterprise to interact with stakeholders.|
|brand|Stakeholder|EDGY defines brand as a name and what it stands for, which makes it a representation of a group of people, their reputation and actions. In ArchiMate® this is best modelled as a kind of (named) stakeholder.|

## Relationships
EDGY only has three relationship types that can be mapped to similarly generic relations in ArchiMate®, in order to permit flexible modelling.

![EDGY ArchiMate Relationships.png]

|EDGY Relationship|ArchiMate® Relation|Observations|
|---|---|---|
|Link|Association|EDGY's link relationship corresponds to a not further specificed association relation in ArchiMate®. Both languages support undirected relationships, and directed ones as in EDGY's Core Links.|
|Flow|Flow|Both languages have a notion of flow between two elements.|
|Tree|Aggregation|In EDGY any hierarchical representation of the same element is a tree relationship, which corresponds to an aggregation relationship in ArchiMate® as it doesn't further specify the nature of the hierarchy.|

## Usage and customisation
The EDGY diagram notation can be introduced in many ArchiMate® capable tools by simply integrating alternative shapes and colours. Both languages encourage custom visualisations to make maps/views more accessible and appealing.

To allow adaptation to a specific context of use, EDGY features a Labels concept to further distinguish elements and capture additional information. With ArchiMate® as underlying modelling language this can be implemented as follows:

- For tags differentiating different types of an element, further ArchiMate® specialisations beyond this mapping can be defined.
- Depending on the tool support this can also be an attribute stored with the element in a repository, or a simple graphical overlay. This also applies to added metrics.

![EDGY-ArchiMate-Mapping-Labels.png]
Examples of custom mappings

If you consider using this mapping from EDGY to ArchiMate™ in your work or tools, join our community to exchange with peers and get involved in its further development.


---
特に断りのない限り、コンテンツはCC BY-SA 4.0ライセンスの下で利用可能です。
