# aem.live Content Map — Core Pages

A filtered view of [catalog-full.md](catalog-full.md): only pages classified as **level = core** (the mainstream path through Edge Delivery Services documentation, excluding `advanced`, `reference`, and `legacy` material). Same structure and schema as the full catalog — just narrower.

## Schema

| Field | Meaning |
|---|---|
| **Title** | Page title (linked to the public URL) |
| **Audience** | Who the page is primarily written for: `author`, `developer`, or `business` |
| **Level** | Always `core` in this file (see [catalog-full.md](catalog-full.md) for `advanced`, `reference`, `legacy`) |
| **Type** | `overview`, `tutorial`, `guide`, `reference`, `faq` |
| **Description** | One-sentence, neutral summary of the page's content |

## Taxonomy

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

## 3. Authoring

Document Authoring, Word/SharePoint, Google Drive, Sidekick and author-facing workflows.

| Title | Audience | Level | Type | Description |
|---|---|---|---|---|
| [Authoring and Publishing Content](https://www.aem.live/docs/authoring) | author | core | guide | Guide explaining how to create website content using Word or Google Docs, add images and videos, create links, use blocks for structured content, and preview or publish pages using the Sidekick tool. |
| [How to use Adobe Sharepoint](https://www.aem.live/docs/setup-adobe-sharepoint) | developer | core | guide | Provides instructions for setting up an Adobe SharePoint instance as a website root, including sharing access and configuring the fstab.yaml file. |
| [How to use Google Drive](https://www.aem.live/docs/setup-googledrive) | developer | core | guide | Explains how to configure Google Drive access for an Edge Delivery Services site, offering either a default Adobe user or custom user setup options. |
| [How to use Sharepoint](https://www.aem.live/docs/setup-sharepoint) | developer | core | overview | Provides guidance on setting up SharePoint access depending on whether content is hosted on Adobe's platform or a customer's non-Adobe instance. |
| [Using AEM Sidekick](https://www.aem.live/docs/sidekick) | author | core | guide | Covers the AEM Sidekick browser extension, including installation, core features like environment switching and content publishing, bulk actions, and project configuration options. |
| [Setup Google Drive as a Content Source](https://www.aem.live/developer/setup-google-drive) | developer | core | guide | Explains how to connect a Google Drive folder containing documents and spreadsheets as a content source for an AEM project, including installation of the Sidekick extension for previewing and publishing content. |

## 4. AEM & Universal Editor

AEM authoring, Universal Editor, component definitions/models, AEM Assets and AEM-specific publishing.

| Title | Audience | Level | Type | Description |
|---|---|---|---|---|
| [Authoring with AEM Sites for Edge Delivery Services](https://www.aem.live/docs/aem-authoring) | author | core | overview | Guide to using AEM as a Cloud Service with the Universal Editor to author and manage content that is delivered through Edge Delivery Services for high performance. |
| [How content is published from AEM Sites authoring to Edge Delivery Services](https://www.aem.live/docs/publishing-from-authoring) | developer | core | guide | Explains the automated workflow that occurs when an author publishes content through the Universal Editor, detailing the process from publication through content ingestion. |
| [Content modeling for AEM authoring projects](https://www.aem.live/developer/component-model-definitions) | developer | core | guide | Explains how to model content for Adobe Experience Manager (AEM) authoring projects using Edge Delivery Services, covering default content, blocks, sections, and metadata configuration. |
| [Set Up AEM Sites as a Content Source](https://www.aem.live/developer/ue-tutorial) | developer | core | tutorial | A tutorial guiding users through creating an Adobe Experience Manager project with Universal Editor, connecting it to a GitHub repository, and publishing content to Edge Delivery Services. |

## 5. Project Anatomy

Repository structure, scripts, styles, configuration files/services and runtime conventions.

| Title | Audience | Level | Type | Description |
|---|---|---|---|---|
| [The Anatomy of a Project](https://www.aem.live/developer/anatomy-of-a-project) | developer | core | overview | This document explains the structure and components of a typical Adobe Experience Manager project, including Git repository setup, special files like head.html and 404.html, configuration management, and commonly-used folder structures for scripts, styles, and blocks. |
| [Favicon](https://www.aem.live/developer/favicon) | developer | core | guide | Instructions for adding a favicon to your website, including methods for code repositories, repoless setups, and AEM Authoring content sources. |

## 6. Blocks & Markup

Blocks, sections, default content, semantic markup, decoration and Block Collection.

| Title | Audience | Level | Type | Description |
|---|---|---|---|---|
| [David's Model, Second take.](https://www.aem.live/docs/davidsmodel) | developer | core | guide | A collection of 15 content modeling best practices for Adobe Experience Manager focused on creating intuitive authoring experiences across different platforms. |
| [Exploring blocks](https://www.aem.live/docs/exploring-blocks) | developer | core | guide | Explains how to create and customize blocks, foundational structural components built from tables in Google Docs or Word that are converted to HTML divs and enhanced with CSS and JavaScript for form and functionality. |
| [Block Collection](https://www.aem.live/developer/block-collection) | developer | core | overview | This page documents AEM's collection of reusable content blocks organized into boilerplate and block collection tiers, with technical principles emphasizing intuitiveness, responsiveness, and accessibility. |
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
| [Page Metadata](https://www.aem.live/docs/metadata) | author | core | guide | Explains how to add invisible page metadata using table-based formatting to help search engines and social media sites understand and categorize content. |
| [Redirects](https://www.aem.live/docs/redirects) | developer | core | guide | Explains how to manage website redirects using a spreadsheet, including redirect precedence, wildcard redirects at the CDN level, and SEO considerations for site migrations. |
| [SEO & GEO Best Practices](https://www.aem.live/docs/seo-geo) | developer | core | guide | Provides guidance on search engine optimization and crawler indexing in AEM, covering rendering approaches, site structure, and results from a server-side rendering experiment. |
| [Indexing](https://www.aem.live/developer/indexing) | developer | core | guide | Adobe Experience Manager provides indexing capabilities to maintain an index of published pages, supporting search, filtering, and list/feed generation through JSON delivery and spreadsheet-based indexing. |
| [Sitemaps](https://www.aem.live/developer/sitemap) | developer | core | guide | AEM can automatically generate sitemap files in three ways—without configuration, based on query indexes, or through manual configuration—to help with SEO and content discovery, with support for multiple languages and hreflang references. |

## 9. Development & Performance

Local development, CLI, developer workflow, performance, Core Web Vitals, testing and coding practices.

| Title | Audience | Level | Type | Description |
|---|---|---|---|---|
| [Development Collaboration and Good Practices](https://www.aem.live/docs/dev-collab-and-good-practices) | developer | core | guide | A guide to collaborative development practices for AEM projects, covering GitHub workflows, CSS and JavaScript standards, and content-first development approaches. |
| [Web Performance, Keeping your Lighthouse Score 100](https://www.aem.live/developer/keeping-it-100) | developer | core | guide | Explains how to maintain a perfect Lighthouse score of 100 by optimizing web performance through server-side rendering, three-phase loading strategies, and avoiding common performance anti-patterns. |

## 10. Configuration & APIs

Configuration Service, Admin API, configuration tooling and other APIs.

| Title | Audience | Level | Type | Description |
|---|---|---|---|---|
| [Setting up the configuration service](https://www.aem.live/docs/config-service-setup) | developer | core | guide | Explains how to set up and manage AEM's configuration service, which aggregates configuration for various consumers and supports multiple sites sharing the same code repository through REST API calls. |
| [Configuration templates](https://www.aem.live/docs/configuration-templates) | developer | core | guide | Guide for creating and managing project configurations using AEM Sites console with support for inheritance across sites via Multi-site management. |

## 11. Git & Environments

Git, GitHub, BYO Git, branches, staging, preview environments and deployment workflows.

| Title | Audience | Level | Type | Description |
|---|---|---|---|---|
| [Staging & Environments](https://www.aem.live/docs/staging) | developer | core | guide | Explains when and how to implement staging environments for AEM development, arguing most teams don't need dedicated staging but recommending staging CDN setups for complex configurations. |
| [Bring Your Own Git](https://www.aem.live/developer/byo-git) | developer | core | guide | Explains how to configure external Git repositories (GitHub Enterprise, BitBucket, GitLab, Azure DevOps) with Adobe Cloud Manager for Edge Delivery Services deployment. |

## 12. Integrations

Adobe and third-party integrations, Forms, analytics, BYOM, JSON2HTML and related integration patterns.

| Title | Audience | Level | Type | Description |
|---|---|---|---|---|
| [Integrations Overview](https://www.aem.live/docs/integrations) | developer | core | overview | A guide to Adobe Experience Manager's integrations with various technologies including CDNs, authoring tools, marketing platforms, and development services. |
| [Forms](https://www.aem.live/developer/forms) | developer | core | overview | Edge Delivery Services for AEM Forms enables rapid creation and deployment of forms using document-based or WYSIWYG authoring, with features like spreadsheet integration and performance monitoring. |
| [Configuring Google Analytics & Tag Manager Integration](https://www.aem.live/developer/gtm-martech-integration) | developer | core | guide | Explains how to set up Google Analytics 4 and Google Tag Manager integration with AEM Edge Delivery Services, including installation, configuration, testing, and privacy compliance steps. |
| [Configuring Adobe Experience Cloud Integration](https://www.aem.live/developer/martech-integration) | developer | core | guide | Guide for setting up integration with Adobe's marketing technology stack including Experience Platform WebSDK, Analytics, Target, Journey Optimizer, and Tags for personalization and tracking. |
| [Configuring Adobe Target Integration](https://www.aem.live/developer/target-integration) | developer | core | guide | Provides step-by-step instructions for integrating Adobe Target with a website using either the Adobe Experience Platform WebSDK or the legacy at.js approach to enable personalization through the Visual Experience Composer. |

## 13. CDN, Caching & Delivery

CDN setup, Adobe-managed CDN, Cloudflare, Akamai, Fastly, CloudFront, caching, invalidation, DNS and domains.

| Title | Audience | Level | Type | Description |
|---|---|---|---|---|
| [Adobe Managed CDN](https://www.aem.live/docs/byo-cdn-adobe-managed) | developer | core | guide | Instructions for configuring Adobe Managed CDN to deliver content from Edge Delivery Services sites, including prerequisites, deployment options, and DNS setup procedures. |
| [Akamai Setup](https://www.aem.live/docs/byo-cdn-akamai-setup) | developer | core | guide | Instructions for configuring Akamai Property Manager to deliver AEM content through an Akamai CDN, including essential settings for origin server, caching, headers, and behaviors. |
| [Cloudflare Setup](https://www.aem.live/docs/byo-cdn-cloudflare-worker-setup) | developer | core | guide | Instructions for configuring Cloudflare to deliver content, including DNS setup, SSL/TLS configuration, caching rules, and Cloudflare Workers deployment. |
| [Amazon Web Services (AWS) CloudFront Setup](https://www.aem.live/docs/byo-cdn-cloudfront-setup) | developer | core | guide | Instructions for configuring AWS CloudFront to deliver content from an AEM origin, including cache policies, origin request policies, distribution creation, and custom header configuration. |
| [Fastly Setup](https://www.aem.live/docs/byo-cdn-fastly-setup) | developer | core | guide | Instructions for configuring Fastly CDN to deliver content, including domain setup, origin configuration, VCL snippets, and optional authentication. |
| [BYO CDN Setup](https://www.aem.live/docs/byo-cdn-setup) | developer | core | overview | Guide for configuring a customer-owned CDN to deliver AEM content, including required settings and vendor-specific setup instructions for Cloudflare, Akamai, Fastly, and CloudFront. |
| [Picking the right CDN](https://www.aem.live/docs/cdn-guide) | developer | core | guide | Guide to selecting a Content Delivery Network for Adobe Experience Manager, comparing options including Fastly, Cloudflare, Cloudfront, and Akamai. |

## 14. Security

Security architecture, authentication, authorization and access control.

| Title | Audience | Level | Type | Description |
|---|---|---|---|---|
| [Authentication Overview](https://www.aem.live/docs/authentication-setup) | developer | core | overview | Outlines authentication options for aem.live, covering setup methods for both visitor access to sites and author access through Sidekick and the Admin API. |
| [Configuring Authentication for Authors](https://www.aem.live/docs/authentication-setup-authoring) | developer | core | guide | Explains how to enable authentication for authors in AEM via Sidekick by configuring access statements, managing user roles, and setting up permissions through the admin service. |
| [Configuring Site Authentication](https://www.aem.live/docs/authentication-setup-site) | developer | core | guide | Instructions for enabling token-based authentication on AEM Live sites using the Configuration Service API to protect preview and publish environments. |
| [Security Overview](https://www.aem.live/docs/security) | developer | core | overview | Details the security architecture and practices for AEM Edge Delivery Services, covering tenant isolation, encryption, authentication, rate limiting, and compliance certifications. |
| [Site authentication for your visitors when using AEM Authoring](https://www.aem.live/developer/authentication-setup-site-for-aem-authoring) | developer | core | guide | This guide explains how to configure token-based site authentication in AEM authoring environments to protect preview and publish sites. |

## 15. Launch & Operations

Go-live, production readiness, monitoring, operational procedures and troubleshooting.

| Title | Audience | Level | Type | Description |
|---|---|---|---|---|
| [Error Pages](https://www.aem.live/docs/error-pages) | developer | core | guide | Documentation on configuring error pages in Adobe Experience Manager, with specific guidance on handling 404 errors and customizing error content using fragments. |
| [Go-Live Checklist](https://www.aem.live/docs/go-live-checklist) | developer | core | guide | A comprehensive checklist of best practices and validation steps to perform before and after launching a website on Adobe Experience Manager. |
| [Operational Telemetry](https://www.aem.live/docs/operational-telemetry) | developer | core | overview | Explains the telemetry system that gathers operations data needed to discover and fix functional and performance issues, emphasizing privacy protections through sampling and data minimization. |
| [Operations](https://www.aem.live/docs/operations) | developer | core | overview | Outlines the operational practices, infrastructure resilience, monitoring systems, and shared responsibilities for maintaining Edge Delivery Services. |
| [Scheduling](https://www.aem.live/docs/scheduling) | developer | core | guide | Explains how to configure and use AEM's task scheduling system to execute actions like previewing, publishing, and purging pages at specified times via a crontab configuration sheet. |
| [Scheduled Publishing](https://www.aem.live/developer/scheduling) | developer | core | guide | Explains how to register your organization and site with Edge Delivery Services to enable scheduling of snapshots and individual pages for future publication. |
