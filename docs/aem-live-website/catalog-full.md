# aem.live Content Map

A structured knowledge map of [www.aem.live](https://www.aem.live/), Adobe's documentation site for Edge Delivery Services (EDS). This catalog was built by crawling all 181 pages reachable from the site's sitemap, then classifying each one — it does **not** mirror aem.live's own navigation.

## Schema

Every documentation entry below is captured with:

| Field | Meaning |
|---|---|
| **Title** | Page title (linked to the public URL) |
| **Audience** | Who the page is primarily written for: `author`, `developer`, or `business` |
| **Level** | `core` (mainstream path), `advanced` (specialized/complex scenarios), `reference` (lookup material, not narrative), `legacy` (superseded or deprecated approach) |
| **Type** | `overview`, `tutorial`, `guide`, `reference`, `faq` |
| **Description** | One-sentence, neutral summary of the page's content |

## Taxonomy

Pages are grouped into 15 normalized categories reflecting what the content is actually about, regardless of where it lives in aem.live's URL structure (`/docs/`, `/developer/`, etc. are freely mixed within a category below). A final [Other content](#other-content-non-documentation) section catalogs the non-documentation pages (blog, business/marketing, community, navigation fragments) found during the crawl, for completeness.

1. [Start Here](#1-start-here)
2. [Architecture](#2-architecture)
3. [Authoring](#3-authoring)
4. [AEM & Universal Editor](#4-aem--universal-editor)
5. [Project Anatomy](#5-project-anatomy)
6. [Blocks & Markup](#6-blocks--markup)
7. [Content & Structured Data](#7-content--structured-data)
8. [Metadata, SEO & Search](#8-metadata-seo--search)
9. [Development & Performance](#9-development--performance)
10. [Configuration & APIs](#10-configuration--apis)
11. [Git & Environments](#11-git--environments)
12. [Integrations](#12-integrations)
13. [CDN, Caching & Delivery](#13-cdn-caching--delivery)
14. [Security](#14-security)
15. [Launch & Operations](#15-launch--operations)

---

## 1. Start Here

Tutorials, onboarding, orientation and introductory material.

| Title | Audience | Level | Type | Description |
|---|---|---|---|---|
| [Documentation](https://www.aem.live/docs/) | everyone | core | overview | Comprehensive guides for Adobe Experience Manager covering build, publish, and launch workflows with developer resources and architecture best practices. |
| [Where to author your site](https://www.aem.live/docs/authoring-guide) | author | core | overview | Outlines the content authoring options available for Edge Delivery Services, including Document Authoring, SharePoint, Google Drive, and AEM Universal Editor. |
| [Frequently Asked Questions](https://www.aem.live/docs/faq) | everyone | core | faq | A comprehensive FAQ covering Edge Delivery Services features, architecture, authoring options, development workflows, integrations, and best practices for building fast websites. |
| [Feature Lifecycle](https://www.aem.live/docs/lifecycle) | everyone | core | overview | Explains Edge Delivery Services' feature lifecycle approach, which progresses features through stages from "Map of Interest" to "Product Feature" to "Deprecation" based on customer usage. |
| [Slack](https://www.aem.live/docs/slack) | everyone | core | overview | Explains that Adobe provides dedicated Slack channels for AEM customers where the Adobe team answers questions about launches, migrations, authoring, and development practices. |
| [Teams](https://www.aem.live/docs/teams) | everyone | core | overview | Explains how Adobe creates dedicated Microsoft Teams channels for AEM customers to provide support for authoring, development, and migration questions during business hours. |
| [Getting Started – Developer Tutorial](https://www.aem.live/developer/tutorial) | developer | core | tutorial | A tutorial that guides developers through setting up a new Adobe Experience Manager (AEM) project in 10-20 minutes, covering repository creation, content authoring, and local development. |
| [Welcome! Let's Dive Deeper: Your Next Steps After Watching Our YouTube Video](https://www.aem.live/developer/tutorial-from-youtube) | developer | core | tutorial | A tutorial for setting up an Adobe Experience Manager project using the boilerplate template, connecting a Google Drive content source, and deploying a website in 10-20 minutes. |
| [Accelerate your tutorial with a pre-built environment](https://www.aem.live/developer/ue-trial) | developer | core | overview | Offers users the ability to request a pre-configured AEM Sites tutorial environment to skip manual setup and immediately begin learning about Edge Delivery Services, content management, and Universal Editor. |

## 2. Architecture

System architecture, content/code separation, delivery architecture, availability and fundamental EDS concepts.

| Title | Audience | Level | Type | Description |
|---|---|---|---|---|
| [Architecture](https://www.aem.live/docs/architecture) | developer | core | overview | Explains Adobe Experience Manager's composable architecture, including how Edge Delivery Services integrates with CDNs, the four-layer technical stack, and the publishing workflow for content, media, code, and configuration. |
| [Global Availability](https://www.aem.live/docs/global) | developer | core | overview | Edge Delivery Services uses redundant global CDNs and distributed points of presence to ensure high availability and low latency for Adobe Experience Manager sites worldwide. |
| [Large Sites](https://www.aem.live/docs/large-sites) | developer | advanced | guide | This guide outlines technical limits, scaling challenges, and recommended architectural approaches for building and managing very large websites in AEM, including structuring strategies for sites up to 1 million pages. |
| [Limits](https://www.aem.live/docs/limits) | developer | reference | reference | This page documents system limits across multiple dimensions including delivery, content source, GitHub sync, and API operations to ensure stability and prevent misuse. |
| [Network Profile](https://www.aem.live/docs/network-profile) | developer | advanced | reference | Documents the network architecture, DNS scheme, HTTP specifications, caching headers, and API endpoints for AEM Delivery services infrastructure. |
| [Repoless - One codebase, many sites](https://www.aem.live/docs/repoless) | developer | advanced | overview | Explains how to create and manage multiple websites that share the same codebase but use different content sources through AEM's Configuration Service. |
| [Folder Mapping](https://www.aem.live/developer/folder-mapping) | developer | legacy | guide | Folder mapping allows a single page to serve content for multiple URLs, but it's only recommended for authenticated sites or single-page apps and should be avoided for SEO-focused content due to creating infinite URL spaces. |

## 3. Authoring

Document Authoring, Word/SharePoint, Google Drive, Sidekick and author-facing workflows.

| Title | Audience | Level | Type | Description |
|---|---|---|---|---|
| [Adobe Experience Manager Assets Sidekick Plugin](https://www.aem.live/docs/aem-assets-sidekick-plugin) | author | advanced | guide | A plugin that allows content authors to access and insert assets from Experience Manager Assets repositories while authoring documents in Microsoft Word or Google Docs. |
| [Authoring and Publishing Content](https://www.aem.live/docs/authoring) | author | core | guide | Guide explaining how to create website content using Word or Google Docs, add images and videos, create links, use blocks for structured content, and preview or publish pages using the Sidekick tool. |
| [How to use Adobe Sharepoint](https://www.aem.live/docs/setup-adobe-sharepoint) | developer | core | guide | Provides instructions for setting up an Adobe SharePoint instance as a website root, including sharing access and configuring the fstab.yaml file. |
| [How to use Google Drive with a custom user](https://www.aem.live/docs/setup-customer-googledrive) | developer | advanced | guide | Explains how to set up a technical user account to access Google Drive content through an AEM service, including folder creation, user sharing, and registration steps. |
| [How to use Sharepoint (application)](https://www.aem.live/docs/setup-customer-sharepoint) | developer | advanced | guide | Explains how to set up SharePoint as a content source for AEM by configuring Microsoft Azure application permissions to access SharePoint sites securely. |
| [How to use Sharepoint (delegated)](https://www.aem.live/docs/setup-customer-sharepoint-user) | developer | advanced | guide | Provides instructions for setting up delegated permissions allowing AEM to access SharePoint content on behalf of a registered user, including Azure application registration steps. |
| [How to use Google Drive](https://www.aem.live/docs/setup-googledrive) | developer | core | guide | Explains how to configure Google Drive access for an Edge Delivery Services site, offering either a default Adobe user or custom user setup options. |
| [How to use Sharepoint](https://www.aem.live/docs/setup-sharepoint) | developer | core | overview | Provides guidance on setting up SharePoint access depending on whether content is hosted on Adobe's platform or a customer's non-Adobe instance. |
| [Using AEM Sidekick](https://www.aem.live/docs/sidekick) | author | core | guide | Covers the AEM Sidekick browser extension, including installation, core features like environment switching and content publishing, bulk actions, and project configuration options. |
| [AEM Sidekick Errors](https://www.aem.live/docs/sidekick-errors) | author | reference | reference | Documents all error messages that can appear in AEM Sidekick, listing the likely causes for each issue. |
| [What is the Sidekick Library?](https://www.aem.live/docs/sidekick-library) | developer | advanced | guide | Explains how to set up and use the Sidekick Library, an AEM extension enabling developers to create UI tools for content authors, including a built-in blocks plugin and custom plugin development. |
| [Configuring Adobe Experience Manager Assets Sidekick Plugin](https://www.aem.live/developer/configuring-aem-assets-sidekick-plugin) | developer | advanced | guide | Explains how to configure the Adobe Experience Manager Assets Sidekick plugin to enable access to assets from your Experience Manager repository while authoring documents in Microsoft Word or Google Docs. |
| [Setup Google Drive as a Content Source](https://www.aem.live/developer/setup-google-drive) | developer | core | guide | Explains how to connect a Google Drive folder containing documents and spreadsheets as a content source for an AEM project, including installation of the Sidekick extension for previewing and publishing content. |
| [Extending the Sidekick](https://www.aem.live/developer/sidekick-development) | developer | advanced | guide | Explains how developers can interact with and customize the AEM sidekick by listening to events, configuring plugins, and creating special views for their projects. |
| [Migrating Your Sidekick v6 Customizations](https://www.aem.live/developer/sidekick-v7-migration) | developer | legacy | guide | Guide for developers on updating custom code from Sidekick v6 to v7, including changes to element names, event names, and event payload structures. |

## 4. AEM & Universal Editor

AEM authoring, Universal Editor, component definitions/models, AEM Assets and AEM-specific publishing.

| Title | Audience | Level | Type | Description |
|---|---|---|---|---|
| [Authoring with AEM Sites for Edge Delivery Services](https://www.aem.live/docs/aem-authoring) | author | core | overview | Guide to using AEM as a Cloud Service with the Universal Editor to author and manage content that is delivered through Edge Delivery Services for high performance. |
| [Managing tabular data with AEM authoring as your content source](https://www.aem.live/docs/authoring-tabular-data) | author | advanced | guide | Explains how to create and manage spreadsheets in AEM with Edge Delivery Services to store tabular data like redirects, metadata, and configurations that are converted to JSON files. |
| [Managing taxonomy data with AEM authoring as your content source](https://www.aem.live/docs/authoring-taxonomy) | author | advanced | guide | Explains how to create, edit, and publish taxonomy pages in AEM to organize tags for use with the Universal Editor, including configuration steps and JSON access methods. |
| [How content is published from AEM Sites authoring to Edge Delivery Services](https://www.aem.live/docs/publishing-from-authoring) | developer | core | guide | Explains the automated workflow that occurs when an author publishes content through the Universal Editor, detailing the process from publication through content ingestion. |
| [Publishing pages with AEM Assets](https://www.aem.live/docs/universal-editor-assets) | developer | advanced | guide | Explains how to configure AEM Assets and Edge Delivery Services to publish assets alongside content, covering folder accessibility, configuration assignment, and asset resizing requirements. |
| [Explore new AI workflows in AEM](https://www.aem.live/developer/aem-playground) | developer | advanced | overview | This page offers access to a temporary playground environment where users can test five AI agents designed to automate content generation, brand compliance, media optimization, and site performance within Adobe Experience Manager. |
| [Path mapping for AEM authoring as your content source](https://www.aem.live/developer/authoring-path-mapping) | developer | advanced | guide | This page explains how to configure path mapping in Adobe Experience Manager to control how content moves between AEM authoring instances and public Edge Delivery Services websites. |
| [Content modeling for AEM authoring projects](https://www.aem.live/developer/component-model-definitions) | developer | core | guide | Explains how to model content for Adobe Experience Manager (AEM) authoring projects using Edge Delivery Services, covering default content, blocks, sections, and metadata configuration. |
| [Publishing AEM Content Fragments to Edge Delivery Services](https://www.aem.live/developer/content-fragment-overlay) | developer | advanced | guide | A guide for publishing Adobe Experience Manager content fragments as self-contained semantic HTML to Edge Delivery Services, enabling better LLM optimization and omnichannel delivery through the json2html service. |
| [Reusing code across sites with AEM authoring as your content source](https://www.aem.live/developer/repoless-authoring) | developer | advanced | guide | Explains how to activate and configure the "repoless" feature in AEM, enabling multiple sites to share the same codebase while sourcing content from AEM authoring. |
| [Repoless stage and prod environments with AEM authoring as your content source](https://www.aem.live/developer/repoless-environments) | developer | advanced | guide | Documentation for setting up separate staging and production environments in Edge Delivery Services using AEM as the content source, including configuration steps and verification procedures. |
| [Multi site management with AEM authoring as your content source](https://www.aem.live/developer/repoless-multisite-manager) | developer | advanced | guide | Explains how to configure Multi Site Manager (MSM) with Edge Delivery Services to manage localized site content across multiple regions while sharing a central codebase. |
| [Set Up AEM Sites as a Content Source](https://www.aem.live/developer/ue-tutorial) | developer | core | tutorial | A tutorial guiding users through creating an Adobe Experience Manager project with Universal Editor, connecting it to a GitHub repository, and publishing content to Edge Delivery Services. |
| [Creating Blocks Instrumented for use with the Universal Editor](https://www.aem.live/developer/universal-editor-blocks) | developer | advanced | guide | A guide for creating and styling blocks for the Universal Editor in AEM, including defining block structures, adding content, implementing decoration and styles, and supporting both AEM and document-based authoring. |

## 5. Project Anatomy

Repository structure, scripts, styles, configuration files/services and runtime conventions.

| Title | Audience | Level | Type | Description |
|---|---|---|---|---|
| [The Anatomy of a Project](https://www.aem.live/developer/anatomy-of-a-project) | developer | core | overview | This document explains the structure and components of a typical Adobe Experience Manager project, including Git repository setup, special files like head.html and 404.html, configuration management, and commonly-used folder structures for scripts, styles, and blocks. |
| [Favicon](https://www.aem.live/developer/favicon) | developer | core | guide | Instructions for adding a favicon to your website, including methods for code repositories, repoless setups, and AEM Authoring content sources. |
| [Change Site Root](https://www.aem.live/developer/change-site-root) | developer | advanced | guide | Instructions for relocating an AEM Boilerplate project's document root to a subpage by reorganizing files in document storage and code, updating file paths accordingly. |

## 6. Blocks & Markup

Blocks, sections, default content, semantic markup, decoration and Block Collection.

| Title | Audience | Level | Type | Description |
|---|---|---|---|---|
| [David's Model, Second take.](https://www.aem.live/docs/davidsmodel) | developer | core | guide | A collection of 15 content modeling best practices for Adobe Experience Manager focused on creating intuitive authoring experiences across different platforms. |
| [Exploring blocks](https://www.aem.live/docs/exploring-blocks) | developer | core | guide | Explains how to create and customize blocks, foundational structural components built from tables in Google Docs or Word that are converted to HTML divs and enhanced with CSS and JavaScript for form and functionality. |
| [Widgets](https://www.aem.live/docs/widgets) | developer | advanced | guide | Explains how to create and use widgets, self-contained application components with their own HTML, CSS, and JavaScript that can be embedded in pages via URL references. |
| [Block Collection](https://www.aem.live/developer/block-collection) | developer | core | overview | This page documents AEM's collection of reusable content blocks organized into boilerplate and block collection tiers, with technical principles emphasizing intuitiveness, responsiveness, and accessibility. |
| [Breadcrumbs](https://www.aem.live/developer/block-collection/breadcrumbs) | developer | reference | reference | Breadcrumbs are navigational UI components that display a list of page titles and relevant links showing the location of the current page in the navigational hierarchy. |
| [Buttons](https://www.aem.live/developer/block-collection/buttons) | developer | reference | reference | This page documents how buttons are implemented in the Boilerplate project, using bold and italic tags to define primary and secondary button variations styled through CSS. |
| [Code](https://www.aem.live/developer/block-collection/code) | developer | reference | reference | This page documents how to display code elements, both inline and multiline, in technical documentation, explaining that fixed-font formatting automatically generates appropriate HTML code blocks. |
| [Footer (Block)](https://www.aem.live/developer/block-collection/footer) | developer | reference | reference | This page documents the Footer block component, which is automatically loaded into the footer element of pages and provides a reusable template for site-wide footer content. |
| [Header (Block)](https://www.aem.live/developer/block-collection/header) | developer | reference | reference | This page documents the header block component, which is automatically loaded into the header element of pages and provides responsive navigation functionality structured around branding, navigation sections, and tools. |
| [Headings](https://www.aem.live/developer/block-collection/headings) | developer | reference | reference | This page explains how to use semantic heading hierarchies (H1-H6) in documents, emphasizing that each page should have only one H1 and headings must follow a proper sequential structure. |
| [Icons](https://www.aem.live/developer/block-collection/icons) | developer | reference | reference | This page explains how to reference and implement icons in web content using the `:<iconname>:` notation, supporting CSS classes, icon fonts, and SVG implementations. |
| [Images](https://www.aem.live/developer/block-collection/images) | developer | reference | reference | This page provides guidance on incorporating images into web documents, including recommendations for resolution, alt-text accessibility, and how the AEM system automatically optimizes images for different browsers and displays. |
| [Links](https://www.aem.live/developer/block-collection/links) | developer | reference | reference | This page explains how to create and implement hyperlinks in web content, including technical guidance on handling internal/external links and workarounds for linking constraints in Microsoft Word Online. |
| [Lists](https://www.aem.live/developer/block-collection/lists) | developer | reference | reference | This page explains how lists are implemented in web content, covering the conversion of numbered and bullet lists to HTML `<ol>` and `<ul>` tags, along with recommendations for maintaining simplicity in list structure. |
| [Metadata Block](https://www.aem.live/developer/block-collection/metadata) | developer | reference | reference | This documentation page explains how the Metadata table works in the pipeline service, detailing how it adds meta tags to HTML markup and describing its name/value pair structure with special properties. |
| [Modal](https://www.aem.live/developer/block-collection/modal) | developer | reference | reference | A modal is a popup component that appears over site content and requires user interaction to open and close, implemented by linking to a `/modals/` path with accompanying CSS and JavaScript code available in the AEM Block Collection. |
| [Search](https://www.aem.live/developer/block-collection/search) | developer | reference | reference | This page documents a search block component that enables users to find site content through search terms, with implementation code available in the AEM Block Collection repository. |
| [Section Metadata](https://www.aem.live/developer/block-collection/section-metadata) | developer | reference | reference | This page explains how the Section Metadata block adds data attributes to containing sections using name/value pairs, with special handling for Style and Id properties. |
| [Sections](https://www.aem.live/developer/block-collection/sections) | developer | reference | reference | Sections are the top-level grouping mechanism in documents that use horizontal rules to organize content and blocks into logical containers with styling capabilities. |
| [Text](https://www.aem.live/developer/block-collection/text) | developer | reference | reference | Documentation explaining how AEM handles text paragraphs with semantic formatting (bold, italic, underline, etc.) and their conversion to HTML tags. |
| [HTML Markup reference](https://www.aem.live/developer/markup-reference) | developer | reference | reference | Describes the structure of HTML markup rendered by the Franklin pipeline, including metadata, head content, and main content sections with allowed HTML tags. |
| [Markup, Sections, Blocks, and Auto Blocking](https://www.aem.live/developer/markup-sections-blocks) | developer | core | guide | Explains how to structure web content using markup, sections, blocks, and auto blocking to create flexible, author-friendly websites with organized developer code. |

## 7. Content & Structured Data

Spreadsheets, JSON, fragments, Content Fragments, placeholders and structured content.

| Title | Audience | Level | Type | Description |
|---|---|---|---|---|
| [Fragments](https://www.aem.live/docs/fragments) | developer | core | overview | Fragments are reusable chunks of content in AEM Edge Delivery Services that can be authored once and referenced across multiple pages to improve performance and consistency. |
| [Media Assets](https://www.aem.live/docs/media) | developer | core | guide | This page explains how AEM manages and delivers media assets like images and videos through its Media Bus infrastructure, including approaches for centralized asset management and dynamic image manipulation. |
| [Placeholders](https://www.aem.live/docs/placeholders) | author | core | guide | Explains how to manage and use centralized placeholder spreadsheets containing key-value pairs for strings and variables across websites, particularly for multilingual sites. |
| [Using Placeholders](https://www.aem.live/developer/placeholders) | developer | core | guide | Explains how to implement and manage placeholders for strings and variables in websites, particularly for multi-language support, using the `fetchPlaceholders` function. |
| [Spreadsheets and JSON](https://www.aem.live/developer/spreadsheets) | developer | core | guide | AEM converts spreadsheets from content sources into structured JSON data, supporting single-sheet and multi-sheet formats with query parameters for pagination and sheet selection. |

## 8. Metadata, SEO & Search

Metadata, bulk metadata, indexing, search, sitemap, robots, redirects and localization/discovery.

| Title | Audience | Level | Type | Description |
|---|---|---|---|---|
| [Bulk Metadata](https://www.aem.live/docs/bulk-metadata) | author | advanced | guide | Explains how to apply metadata across multiple pages at once using a metadata sheet, including URL pattern matching, property configuration, and hierarchy rules for metadata precedence. |
| [Indexing reference](https://www.aem.live/docs/indexing-reference) | developer | reference | reference | Documents how to define and configure index definitions in helix-query.yaml, including CSS selectors, value extraction functions, and supported expression syntax for web content indexing. |
| [Page Metadata](https://www.aem.live/docs/metadata) | author | core | guide | Explains how to add invisible page metadata using table-based formatting to help search engines and social media sites understand and categorize content. |
| [Redirects](https://www.aem.live/docs/redirects) | developer | core | guide | Explains how to manage website redirects using a spreadsheet, including redirect precedence, wildcard redirects at the CDN level, and SEO considerations for site migrations. |
| [Using Schema (Structured Data) as JSON-LD](https://www.aem.live/docs/schema-structured-data) | developer | advanced | guide | Explains how to implement structured data using JSON-LD in AEM, comparing block-based and page-based approaches and covering testing, measurement, and best practices for search visibility. |
| [SEO & GEO Best Practices](https://www.aem.live/docs/seo-geo) | developer | core | guide | Provides guidance on search engine optimization and crawler indexing in AEM, covering rendering approaches, site structure, and results from a server-side rendering experiment. |
| [Translation and Localization](https://www.aem.live/docs/translation-and-localization) | developer | advanced | guide | Explains best practices for structuring multilingual websites using a language-first approach with market-level fallbacks, covering URL architecture, language detection, and translation handling. |
| [Indexing](https://www.aem.live/developer/indexing) | developer | core | guide | Adobe Experience Manager provides indexing capabilities to maintain an index of published pages, supporting search, filtering, and list/feed generation through JSON delivery and spreadsheet-based indexing. |
| [Sitemaps](https://www.aem.live/developer/sitemap) | developer | core | guide | AEM can automatically generate sitemap files in three ways—without configuration, based on query indexes, or through manual configuration—to help with SEO and content discovery, with support for multiple languages and hreflang references. |

## 9. Development & Performance

Local development, CLI, developer workflow, performance, Core Web Vitals, testing and coding practices.

| Title | Audience | Level | Type | Description |
|---|---|---|---|---|
| [Development Collaboration and Good Practices](https://www.aem.live/docs/dev-collab-and-good-practices) | developer | core | guide | A guide to collaborative development practices for AEM projects, covering GitHub workflows, CSS and JavaScript standards, and content-first development approaches. |
| [Experimentation](https://www.aem.live/docs/experimentation) | developer | advanced | guide | Guide to setting up and running A/B tests on Adobe Experience Manager sites by creating challenger page variants and comparing their performance against control pages. |
| [Load, Performance, and Penetration Testing](https://www.aem.live/docs/testing) | developer | advanced | guide | Explains the differences between three testing disciplines for Edge Delivery Services sites and provides best practices for conducting each type of test. |
| [Developing with AI Tools](https://www.aem.live/developer/ai-coding-agents) | developer | advanced | guide | This guide explains how to configure AI coding agents to work effectively with Adobe Experience Manager Edge Delivery Services by providing project context, search guidance, skills, and specialized tools. |
| [aem Command Line Reference](https://www.aem.live/developer/cli-reference) | developer | reference | reference | Documentation for the Adobe AEM CLI tool, covering installation, usage, and detailed reference for the up, import, and content commands with their respective options. |
| [Font Fallback and CLS](https://www.aem.live/developer/font-fallback) | developer | advanced | guide | A guide to using font fallbacks to prevent Cumulative Layout Shift when loading custom fonts, including details about a Chrome extension tool that computes optimal font scaling. |
| [Importing Content](https://www.aem.live/developer/importer) | developer | advanced | guide | AEM provides tools to import existing website content and convert it into docx files, HTML, or content packages for various authoring methods including document-based authoring and Universal Editor workflows. |
| [Web Performance, Keeping your Lighthouse Score 100](https://www.aem.live/developer/keeping-it-100) | developer | core | guide | Explains how to maintain a perfect Lighthouse score of 100 by optimizing web performance through server-side rendering, three-phase loading strategies, and avoiding common performance anti-patterns. |
| [Developing Operational Telemetry in AEM](https://www.aem.live/developer/operational-telemetry) | developer | advanced | guide | Explains how to implement Operational Telemetry in Adobe Experience Manager to track usage and performance metrics through client-side APIs and predefined checkpoint events. |

## 10. Configuration & APIs

Configuration Service, Admin API, configuration tooling and other APIs.

| Title | Audience | Level | Type | Description |
|---|---|---|---|---|
| [Admin API Keys](https://www.aem.live/docs/admin-apikeys) | developer | reference | reference | Explains how to generate, manage, list, update, and delete API keys for authenticating requests to the Admin Service API. |
| [Audit log](https://www.aem.live/docs/auditlog) | developer | advanced | reference | The audit log records admin and indexing operations in Edge Delivery Services, queryable via an Admin endpoint and accessible to users with author role permissions. |
| [Setting up the configuration service](https://www.aem.live/docs/config-service-setup) | developer | core | guide | Explains how to set up and manage AEM's configuration service, which aggregates configuration for various consumers and supports multiple sites sharing the same code repository through REST API calls. |
| [Document-based Project Configuration](https://www.aem.live/docs/configuration) | developer | legacy | reference | Documents how to configure an AEM project using a document-based configuration file located in `/.helix/config.xlsx` or `/.helix/config`, though the Configuration Service is now recommended instead. |
| [Configuration templates](https://www.aem.live/docs/configuration-templates) | developer | core | guide | Guide for creating and managing project configurations using AEM Sites console with support for inheritance across sites via Multi-site management. |
| [Backend Errors](https://www.aem.live/developer/admin-errors) | developer | reference | reference | This page documents HTTP error codes and templates returned by the Admin Service when backend requests fail, along with their likely root causes. |

## 11. Git & Environments

Git, GitHub, BYO Git, branches, staging, preview environments and deployment workflows.

| Title | Audience | Level | Type | Description |
|---|---|---|---|---|
| [Migrating a VIP project to your own infrastructure](https://www.aem.live/docs/move-project-to-customer-infrastructure) | developer | advanced | guide | Provides step-by-step instructions for moving a VIP project from Adobe's hosted infrastructure to a customer's own GitHub repository and SharePoint environment. |
| [Staging & Environments](https://www.aem.live/docs/staging) | developer | core | guide | Explains when and how to implement staging environments for AEM development, arguing most teams don't need dedicated staging but recommending staging CDN setups for complex configurations. |
| [Bring Your Own Git](https://www.aem.live/developer/byo-git) | developer | core | guide | Explains how to configure external Git repositories (GitHub Enterprise, BitBucket, GitLab, Azure DevOps) with Adobe Cloud Manager for Edge Delivery Services deployment. |
| [Using GitHub Actions to handle Publication Events](https://www.aem.live/developer/github-actions) | developer | advanced | guide | Franklin integrates with GitHub Actions to trigger workflows when pages or sheets are published or unpublished, enabling further integrations through WebHooks, API calls, or other GitHub workflows. |
| [Upgrading to aem.live from hlx.live](https://www.aem.live/developer/upgrade) | developer | legacy | guide | A guide for migrating websites from the deprecated hlx.live domain to the new aem.live domain, including configuration updates and advanced scenarios. |

## 12. Integrations

Adobe and third-party integrations, Forms, analytics, BYOM, JSON2HTML and related integration patterns.

| Title | Audience | Level | Type | Description |
|---|---|---|---|---|
| [Embedding Content in non-AEM experiences](https://www.aem.live/docs/aem-embed) | developer | advanced | guide | Explains how to embed AEM-managed content into external websites and applications using Web Components, including implementation steps and configuration requirements. |
| [Integrations Overview](https://www.aem.live/docs/integrations) | developer | core | overview | A guide to Adobe Experience Manager's integrations with various technologies including CDNs, authoring tools, marketing platforms, and development services. |
| [How to build a Storefront in AEM](https://www.aem.live/docs/storefront) | developer | advanced | overview | Provides an overview of Adobe's Commerce Storefront for Edge Delivery Services and directs readers to resources for creating and managing an e-commerce site within AEM. |
| [Bring Your Own Markup](https://www.aem.live/developer/byom) | developer | advanced | guide | BYOM is an API that enables Edge Delivery Services to accept HTML content from custom sources without requiring content migration. |
| [Adding Your Own Consent Management Platform (CMP)](https://www.aem.live/developer/cmp-integration) | developer | advanced | guide | Guide for replacing the default consent-gating implementation with a real consent management platform, including worked examples for OneTrust and Cookiebot. |
| [Forms](https://www.aem.live/developer/forms) | developer | core | overview | Edge Delivery Services for AEM Forms enables rapid creation and deployment of forms using document-based or WYSIWYG authoring, with features like spreadsheet integration and performance monitoring. |
| [Configuring Google Analytics & Tag Manager Integration](https://www.aem.live/developer/gtm-martech-integration) | developer | core | guide | Explains how to set up Google Analytics 4 and Google Tag Manager integration with AEM Edge Delivery Services, including installation, configuration, testing, and privacy compliance steps. |
| [JSON2HTML for Edge Delivery Services](https://www.aem.live/developer/json2html) | developer | advanced | guide | JSON2HTML is a generic worker that transforms JSON data into HTML pages for Adobe's Edge Delivery Services, requiring minimal setup and no custom deployment. |
| [Configuring Adobe Experience Cloud Integration](https://www.aem.live/developer/martech-integration) | developer | core | guide | Guide for setting up integration with Adobe's marketing technology stack including Experience Platform WebSDK, Analytics, Target, Journey Optimizer, and Tags for personalization and tracking. |
| [Configuring Adobe Target Integration](https://www.aem.live/developer/target-integration) | developer | core | guide | Provides step-by-step instructions for integrating Adobe Target with a website using either the Adobe Experience Platform WebSDK or the legacy at.js approach to enable personalization through the Visual Experience Composer. |
| [Web Components](https://www.aem.live/developer/web-components) | developer | advanced | guide | Web Components are a collection of web standards enabling creation of reusable, modular functionality that can be integrated into Adobe Experience Manager projects. |

## 13. CDN, Caching & Delivery

CDN setup, Adobe-managed CDN, Cloudflare, Akamai, Fastly, CloudFront, caching, invalidation, DNS and domains.

| Title | Audience | Level | Type | Description |
|---|---|---|---|---|
| [Adobe Managed CDN](https://www.aem.live/docs/byo-cdn-adobe-managed) | developer | core | guide | Instructions for configuring Adobe Managed CDN to deliver content from Edge Delivery Services sites, including prerequisites, deployment options, and DNS setup procedures. |
| [Akamai Setup](https://www.aem.live/docs/byo-cdn-akamai-setup) | developer | core | guide | Instructions for configuring Akamai Property Manager to deliver AEM content through an Akamai CDN, including essential settings for origin server, caching, headers, and behaviors. |
| [Cloudflare Setup](https://www.aem.live/docs/byo-cdn-cloudflare-worker-setup) | developer | core | guide | Instructions for configuring Cloudflare to deliver content, including DNS setup, SSL/TLS configuration, caching rules, and Cloudflare Workers deployment. |
| [Cloudflare Setup (with wrangler)](https://www.aem.live/docs/byo-cdn-cloudflare-worker-wrangler-setup) | developer | advanced | guide | Guide for configuring Cloudflare using the wrangler command line interface to deliver AEM content, covering DNS, SSL/TLS, caching, page rules, and worker creation. |
| [Amazon Web Services (AWS) CloudFront Setup](https://www.aem.live/docs/byo-cdn-cloudfront-setup) | developer | core | guide | Instructions for configuring AWS CloudFront to deliver content from an AEM origin, including cache policies, origin request policies, distribution creation, and custom header configuration. |
| [Fastly Setup](https://www.aem.live/docs/byo-cdn-fastly-setup) | developer | core | guide | Instructions for configuring Fastly CDN to deliver content, including domain setup, origin configuration, VCL snippets, and optional authentication. |
| [BYO CDN Setup](https://www.aem.live/docs/byo-cdn-setup) | developer | core | overview | Guide for configuring a customer-owned CDN to deliver AEM content, including required settings and vendor-specific setup instructions for Cloudflare, Akamai, Fastly, and CloudFront. |
| [Picking the right CDN](https://www.aem.live/docs/cdn-guide) | developer | core | guide | Guide to selecting a Content Delivery Network for Adobe Experience Manager, comparing options including Fastly, Cloudflare, Cloudfront, and Akamai. |
| [China FAQ](https://www.aem.live/docs/china) | business | advanced | faq | Provides guidance on using Adobe Experience Manager Edge Delivery Services in China, covering content delivery requirements, authoring capabilities, developer experience, and hosting options. |
| [Custom HTTP Response Headers](https://www.aem.live/docs/custom-headers) | developer | advanced | guide | Explains how to apply custom HTTP response headers to resources in site configurations, including CORS headers, with security warnings about access-control-allow-origin settings. |
| [Configuring push invalidation for BYO production CDN](https://www.aem.live/docs/setup-byo-cdn-push-invalidation) | developer | advanced | overview | Explains how to automatically purge cached content from a customer's production CDN when AEM origin content changes on the main branch, with links to vendor-specific setup instructions. |
| [Setup push invalidation for Akamai](https://www.aem.live/docs/setup-byo-cdn-push-invalidation-for-akamai) | developer | advanced | guide | Explains how to configure Akamai Fast Purge credentials to automatically purge cached content when AEM origin content changes on the main branch. |
| [Setup push invalidation for Cloudflare](https://www.aem.live/docs/setup-byo-cdn-push-invalidation-for-cloudflare) | developer | advanced | guide | Explains how to configure automatic cache purging on Cloudflare's CDN when content changes occur on AEM origin servers, including required API token setup. |
| [Set up push invalidation for AWS CloudFront](https://www.aem.live/docs/setup-byo-cdn-push-invalidation-for-cloudfront) | developer | advanced | guide | Explains how to configure automatic content purging on CloudFront CDN when changes are deployed to AEM origins, including creating the necessary AWS IAM credentials. |
| [Setup push invalidation for Fastly](https://www.aem.live/docs/setup-byo-cdn-push-invalidation-for-fastly) | developer | advanced | guide | Explains how to configure Fastly CDN credentials to automatically purge cached content when changes are published to AEM origin branches. |
| [Setup push invalidation for Adobe Managed CDN](https://www.aem.live/docs/setup-byo-cdn-push-invalidation-for-managed) | developer | advanced | guide | Explains how to configure automatic content purging on a production CDN when changes are deployed to AEM origins on the main branch. |
| [Unsupported Integrations](https://www.aem.live/docs/unsupported) | developer | reference | reference | Outlines integration patterns that Adobe discourages for AEM due to security, availability, and performance concerns, including unsupported CDNs, CDN chaining, TLS interception, and certain WAF implementations. |
| [Adobe Managed CDN Advanced Configuration](https://www.aem.live/developer/byo-cdn-adobe-managed-cdn-config) | developer | advanced | guide | Explains how to configure advanced Adobe Managed CDN rules for request/response transformations, traffic filtering, redirects, and authentication mechanisms including Basic Auth and OIDC. |

## 14. Security

Security architecture, authentication, authorization and access control.

| Title | Audience | Level | Type | Description |
|---|---|---|---|---|
| [Authentication Overview](https://www.aem.live/docs/authentication-setup) | developer | core | overview | Outlines authentication options for aem.live, covering setup methods for both visitor access to sites and author access through Sidekick and the Admin API. |
| [Configuring Authentication for Authors](https://www.aem.live/docs/authentication-setup-authoring) | developer | core | guide | Explains how to enable authentication for authors in AEM via Sidekick by configuring access statements, managing user roles, and setting up permissions through the admin service. |
| [Configuring Site Authentication](https://www.aem.live/docs/authentication-setup-site) | developer | core | guide | Instructions for enabling token-based authentication on AEM Live sites using the Configuration Service API to protect preview and publish environments. |
| [Content Security Policy: strict-dynamic + (cached) nonce](https://www.aem.live/docs/csp) | developer | advanced | guide | Guide for implementing a nonce-based Content Security Policy in AEM Edge Delivery Services to mitigate XSS attacks while maintaining CDN caching efficiency. |
| [Security Overview](https://www.aem.live/docs/security) | developer | core | overview | Details the security architecture and practices for AEM Edge Delivery Services, covering tenant isolation, encryption, authentication, rate limiting, and compliance certifications. |
| [AEM Sidekick Security](https://www.aem.live/docs/sidekick-security) | developer | reference | reference | Documents the browser permissions, privacy practices, network requests, and access controls associated with the AEM Sidekick extension. |
| [Site authentication for your visitors when using AEM Authoring](https://www.aem.live/developer/authentication-setup-site-for-aem-authoring) | developer | core | guide | This guide explains how to configure token-based site authentication in AEM authoring environments to protect preview and publish sites. |
| [Cloudflare Zero Trust Site Protection](https://www.aem.live/developer/cloudflare-zero-trust) | developer | advanced | guide | A guide for integrating Cloudflare Zero Trust authentication and authorization to control website access through identity verification and policies. |

## 15. Launch & Operations

Go-live, production readiness, monitoring, operational procedures and troubleshooting.

| Title | Audience | Level | Type | Description |
|---|---|---|---|---|
| [Deprecations and Removals](https://www.aem.live/docs/deprecation) | developer | legacy | reference | Lists AEM features that are deprecated or have been removed, providing end-of-service dates and migration guidance for users. |
| [Error Pages](https://www.aem.live/docs/error-pages) | developer | core | guide | Documentation on configuring error pages in Adobe Experience Manager, with specific guidance on handling 404 errors and customizing error content using fragments. |
| [Go-Live Checklist](https://www.aem.live/docs/go-live-checklist) | developer | core | guide | A comprehensive checklist of best practices and validation steps to perform before and after launching a website on Adobe Experience Manager. |
| [Operational Telemetry](https://www.aem.live/docs/operational-telemetry) | developer | core | overview | Explains the telemetry system that gathers operations data needed to discover and fix functional and performance issues, emphasizing privacy protections through sampling and data minimization. |
| [Operations](https://www.aem.live/docs/operations) | developer | core | overview | Outlines the operational practices, infrastructure resilience, monitoring systems, and shared responsibilities for maintaining Edge Delivery Services. |
| [Service Scaling and High-Visibility Events](https://www.aem.live/docs/peak-traffic) | business | advanced | guide | Explains how Edge Delivery Services maintains automatic scaling through serverless infrastructure and describes optional notification procedures for business-critical traffic events. |
| [Schedule recurring tasks](https://www.aem.live/docs/recurring) | developer | advanced | guide | Explains how to use GitHub Actions to automate recurring tasks, such as publishing an index hourly via a cron schedule and HTTP request action. |
| [Recent Releases](https://www.aem.live/docs/release-history) | developer | reference | reference | Provides a curated list of current AEM component releases sourced from code repositories, noting that some information is public while other details remain internal. |
| [Scheduling](https://www.aem.live/docs/scheduling) | developer | core | guide | Explains how to configure and use AEM's task scheduling system to execute actions like previewing, publishing, and purging pages at specified times via a crontab configuration sheet. |
| [Snapshots and Reviews](https://www.aem.live/docs/snapshots-reviews) | developer | advanced | guide | Explains how content snapshots capture pages at specific points in time for coordinated website launches, enabling review and publication workflows with version-control-like functionality. |
| [Scheduled Publishing](https://www.aem.live/developer/scheduling) | developer | core | guide | Explains how to register your organization and site with Edge Delivery Services to enable scheduling of snapshots and individual pages for future publication. |

---

## Other content (non-documentation)

Pages found during the crawl that are not part of the documentation corpus — marketing/business pages, blog posts, community pages, and navigation fragments. Cataloged for completeness (per the "scrape all sub-pages" requirement) but intentionally excluded from the 15-category taxonomy above.

| Title | Type | Description |
|---|---|---|
| [Adobe Experience Manager](https://www.aem.live/) | landing | Adobe Experience Manager is a content management system that enables fast website creation by integrating with existing tools like Microsoft Office, Google Workspace, and various CDN providers. |
| [AEM.live Blog](https://www.aem.live/blog) | blog | This page curates a collection of links to external blogs and resources focused on Adobe Experience Manager (AEM) content and insights from various industry partners and experts. |
| [Best of adaptTo() 2025](https://www.aem.live/blog/adapt-to-2025) | blog | A recap of notable talks from the 2025 adaptTo() conference, Europe's annual AEM developer event. |
| [aem.live at Adobe Developers Live 2024](https://www.aem.live/blog/aem-live-at-dev-live) | blog | Announces the first in-person Adobe Developers Live event at Adobe's San Jose headquarters. |
| [AEM.live Blog Archive](https://www.aem.live/blog/archive) | blog | Curates a collection of external blog resources and insights related to AEM from various technology organizations and practitioners. |
| [How Edge Delivery Services handles peak season](https://www.aem.live/blog/built-ready-for-the-season) | blog | Explains that Edge Delivery Services requires no special peak season preparation due to its serverless architecture and automatic failover. |
| [The Konami Code for Dynamic Publishing at Scale](https://www.aem.live/blog/byom-content-overlays) | blog | Showcases two developers who published thousands of pages dynamically using Edge Delivery's BYOM and content overlay capabilities. |
| [A Date with Edge Delivery: Putting Calendars on the Web, Twice](https://www.aem.live/blog/calendar-implementation) | blog | Presents two calendar implementation approaches using Edge Delivery Services. |
| [Documents that dazzle, content that clicks, and semantics that snap](https://www.aem.live/blog/content-document-semantics) | blog | Explains the importance of document semantics in AEM content modeling through a hero block example. |
| [The Performance Paradox: When Simple Architecture Beats Complex Frameworks](https://www.aem.live/blog/edge-next) | blog | Compares Edge Delivery Services and Next.js as two architectural approaches to web development. |
| [The One Template That Broke the Internet (And My Heart)](https://www.aem.live/blog/folder-mapping-deprecated) | blog | Explains why folder mapping was deprecated in favor of content overlays. |
| [Bonjour! Hola! Hello! – Creating Multilingual Sites with Ease](https://www.aem.live/blog/future-proof-multilingual-website-edge-ensemble) | blog | Explains how to implement multilingual website support using Edge Delivery Services. |
| [A high-five for aem.live](https://www.aem.live/blog/hlx-is-now-aem-live) | blog | Announces the transition from hlx.live to aem.live domains. |
| [From Signals to Story: Building OpTel Detective](https://www.aem.live/blog/optel-detective) | blog | Explains how OpTel Detective, an AI-powered reporting tool, automates analysis of operational telemetry data. |
| [Unlocking Efficiency with Helix 5](https://www.aem.live/blog/organizing-source-code-ensemble) | blog | Explains how AEM Edge Delivery Services (Helix 5) enables multi-site development from a single shared codebase. |
| [Roadmaps, Marty? Where we're going, we don't need Roadmaps!](https://www.aem.live/blog/roadmaps) | blog | Explains why Edge Delivery Services uses a "feature lifecycle" approach instead of traditional product roadmaps. |
| [AEM Sidekick v7 – The Story Behind the Latest Release](https://www.aem.live/blog/sidekick-v7) | blog | Documents the development history and design improvements behind Sidekick v7. |
| [Why I don't recommend UI testing in AEM](https://www.aem.live/blog/testing-in-aem) | blog | Argues that UI testing in AEM projects typically carries high maintenance costs and low value for most use cases. |
| [The Architecture Problem That's Breaking AIs for Content Management](https://www.aem.live/blog/toms-developer-dilemma) | blog | Explains how traditional CMS architectures create challenges for AI language models and presents a local-first, AI-native framework as a solution. |
| [Increase Content Velocity with Helix](https://www.aem.live/business/content-velocity) | business | Helix streamlines publishing by integrating with existing tools like Word and Google Docs. |
| [Sign up for the VIP Program, Get a Demo](https://www.aem.live/business/demo) | business | Explains that AEM Franklin is available to select customers through a VIP program. |
| [Helix is green](https://www.aem.live/business/helix-is-green) | business | Reports that Helix's page delivery generates 99.4% less CO2 than the global average. |
| [Got Questions? Let's Connect!](https://www.aem.live/business/reachout) | business | Provides information on accessing support resources and requesting consultations. |
| [AEM Community](https://www.aem.live/community) | community | A platform for AEM practitioners to connect through Discord, user groups, and recorded events. |
| [Adobe Developers Live 2026](https://www.aem.live/developers-live) | announcement | Event information for Adobe Developers Live 2026, an online series plus in-person events in San Jose, Basel, Bangalore, and Sydney. |
| [Block Party](https://www.aem.live/developer/block-party/) | community | A community platform where AEM developers can showcase and share reusable blocks, code snippets, and integrations. |
| [Thank you for your submission](https://www.aem.live/developer/block-party/thank-you) | landing | Confirmation page for a Block Party submission. |
| [Thank you for your submission](https://www.aem.live/developer/example-form/thank-you) | landing | Confirmation page for a demonstration form submission. |
| [Getting Started](https://www.aem.live/gnav) | landing | Global navigation fragment providing introductory resources and navigation links for Project Franklin. |
