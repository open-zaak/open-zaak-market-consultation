# Our proposals and questions

| <a href="README.md">Home</a> | <a href="introduction-en.md">Introduction</a> | Our proposals and questions | <a href="how-to-respond-en.md">How to respond</a> |
| -------- | -------- | -------- | -------- |

This page contains three sections:

* Vision for an open source community - a draft vision for what the OpenZaak community could look like
* Needs of municipalities - an indicative overview of kinds of support the municipalities need from vendors
* Market consultation questions - an overview of our open questions to market parties

## Vision for an open source community

We believe the success of OpenZaak involves municipalities and market parties working together towards a common goal: an open and collaborative community at scale.

For municipalities it is important to have a large and diverse vendor network that can support each municipality with their particular needs (including support for development, hosting and implementation). This will also help reduce municipalities’ risks when implementing the OpenZaak codebase.

For vendors it is important to grow the number of replicating municipalities (increasing the market for their services), and to work effectively with other vendors (complementing skill sets and improving the reliability of implementing the OpenZaak codebase).

Without knowing all the answers in detail, our vision for this community includes:

* collaborating on a single, vendor-neutral codebase and shared branching model, avoiding diverging forks
* collaborative governance, including around shared roadmaps (feature and technical) and open issue tracker
* a shared understanding of how to approach bug fixes and support, particularly in situations of operational downtime or security risks
* an inclusive community (including open communication channels, codebase marketing material and codes of conduct) that is welcoming to new market parties and new replicating municipalities
* empowering vendors to become effective members and ambassadors of the community

## Needs of municipalities

OpenZaak consists of a set of components that will be used by a diverse set of municipalities. This means the community needs to be set up to allow for different types of vendors to support different types of municipalities.

The lists below set out needs all municipalities will have, as well as three ‘types’ of municipalities and their corresponding needs vis-à-vis the community and market support.

### Needs all municipalities have

* Need connection with external databases/sets (i.e. basisgegevens)
* Need to retain ownership of data, and continuous access to the data
* Need easy data portability (for example for legally required archiving)
* Need vendors who contribute to the OpenZaak main repository (including [EUPL license](https://github.com/open-zaak/open-zaak/blob/master/LICENSE.md))
* Need to remain in sync with the [VNG standards](https://www.vngrealisatie.nl/producten/api-standaarden-zaakgericht-werken)
* Need to influence the feature roadmap
* Need vendors to use OpenZaak in all products and services that create or use case management data

### ‘Full service’ package needs

Some municipalities need a full service package. This includes hosting, implementation, maintenance and development, by one or many vendors. Additionally, OpenZaak will be integrated with existing products from existing vendors, for example the case management systems they use.

They need market parties to offer:

* hosting support
* implementation support
* maintenance support
* new feature and bug fix support
* integration support
* a helpdesk, configuration support, questions and training
* a way to file bug fixes and deploy hotfixes

### ‘Backend as a service’ needs

Some municipalities need ‘Backend as a service’. They are able to run other applications dependent on OpenZaak on their own servers (or in the cloud), but would like vendors to host, run and maintain OpenZaak for them.

They need market parties to offer:

* an integration partner
* clear continuous integration/continuous development
* a sandbox environment
* a way to file bug fixes and deploy hotfixes
* a helpdesk, configuration support, questions and training

### In-house implementation needs

Some municipalities will want to implement the component with exclusively in-house resources. They will need to coordinate their work with other municipalities and vendors.

They need the community to have:

* clear development/contribution guidelines
* a way to liaise with vendors and other municipalities regarding product and technical roadmap and backlogs
* a way to fix bugs together with vendors and other municipalities

## Market consultation questions

This section includes a list of open questions we have. Each item includes our current assumptions, and open questions we would like to discuss with the vendor community.

Please note questions are indicative - we would love to hear your thoughts on any of the points in this annex.

### 1. Single shared codebase

#### Assumptions

We would like to facilitate an open community at scale, including collaboration on a single, vendor-neutral codebase and shared branching model, avoiding diverging forks. This should be included in the contracts municipalities have with vendors, for example through naming conventions for branches and an emphasis on continuous integration.

#### Questions

1. How would you like to see this principle included in contracts municipalities have with you?
2. How do you propose keeping ‘soft forks’ up to date with each other? Should there be a central repository which can be considered as master?
3. What challenges would working in such a multi-branch environment present for you? How could these challenges be mitigated to reduce the business risks for you?
4. Have you ever worked in this way before?
5. Is the [current architecture and make up of the codebase](https://github.com/open-zaak/open-zaak) conducive to multi-vendor collaboration and modular componentized implementation?

### 2. Shared codebase governance

#### Assumptions

Our vision is to enable collaboration between multiple municipalities and vendors working on the codebase together. For this, we assume we will need shared governance for the codebase. This could include: a) an open shared issue and bug tracker, b) an open and shared feature roadmap, and c) an open and shared technical roadmap. This will also include engineering and contributing guidelines, as well as open communication channels.

This market consultation includes a [draft proposal for a governance structure](governance.md) for open discussion.

#### Questions

1. How would you like to see governance handled within the community?
2. What are the challenges you foresee maintaining open backlogs with your clients?
3. Who should be responsible for updating the shared roadmaps? You, the municipalities, or shared?
4. How would you like to influence the feature and technical roadmap?
5. How would you like to see the community develop, agree and maintain shared engineering and contributing guidelines?
6. What risks do you see working in such an environment?

### 3. Bugs and bug fixes

#### Assumptions

There will be a central, public and prioritised issue tracker for features and bugs. Many of these issues might include small amounts of work (less than 80 hours). Additionally, many municipalities will have issues and bugs related to their local implementation and context.

#### Questions

1. Should work on both local instances and the central repository be included in a single contract?
2. How would you like the contracts to be structured so that you can work on local implementations and branches as well as contributing to the central repository?
3. How should bug fixes be deployed throughout the community? Can vendors take hotfixes from other vendors before these have been merged into the central repository? Or should vendors only implement changes after they have been merged to the central repository?
4. What kind of liability issues can come with hotfixing code that leads to unexpected damage or further problems? Does this create a problem for your contractual obligations to your client?

### 4. Helpdesk and support

#### Assumptions

Many municipalities will prefer to have a single provider they can call for all their needs. This ranges from questions, bugs, ideas for new features, technical integration, training, configuration of permissions/authorisation, notifications, and so forth. Our assumption is that in many cases, no single vendor will want to or be able to provide all these services.

#### Questions

1. Is it possible to set up a single helpdesk to cover everything related to a municipality’s use of OpenZaak? Or are there benefits to different vendors maintaining different helpdesks for different types of questions (for example, to allow them to differentiate their service offering?)
2. Could multiple market parties join together to combine their offering?
3. Could specialised ‘help desk’ providers subcontract work to other providers?

### 5. Standards compliance

#### Assumptions

The OpenZaak APIs are based on the [APIs for zaakgericht werken](https://www.vngrealisatie.nl/producten/api-standaarden-zaakgericht-werken) which is a VNG standard. The standard is continuously maintained and improved, and OpenZaak has to comply with it. These updates will have to be propagated across the central repository branch, as well as repositories that market parties use to deliver their services (like backend-as-a-service).

#### Questions

1. How do we ensure updates to the VNG standard are appropriately reflected across running OpenZaak instances? Should these requirements be included in contracts with market parties?
2. What do you think about version control of OpenZaak vis-à-vis other applications? How many backwards-compatible versions should be supported?
3. Should vendors be asked as part of their contracts to contribute what they’ve learned from implementing and supporting OpenZaak back to the VNG standards?

### 6. Codebase marketing

#### Assumptions

For the community to scale effectively, we assume there should be a set of neutral marketing material, including logo, website, product documentation, case studies, business case material, and so on. We believe this should be vendor -and municipality- neutral to enable a shared set of storytelling resources.

#### Questions

1. How would you like to see this marketing material created?
2. What kind of influence would you like over this material and the website?
3. Should vendors be asked as part of their contracts to contribute what they’ve learned from implementing and supporting OpenZaak to the OpenZaak marketing material (including for example user testimonials, business cases, etc)?

| <a href="README.md">Home</a> | <a href="introduction-en.md">Introduction</a> | Our proposals and questions | <a href="how-to-respond-en.md">How to respond</a> |
| -------- | -------- | -------- | -------- |
