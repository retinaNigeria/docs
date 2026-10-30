# Product brief

## Description
TruHuddle gives organizations a managed blog with branded templates, custom domains and AI-assisted writing.

## Primary audience
Workspace owners and editors publishing company updates, plus developers retrieving published content.

## Jobs to be done
1. Create a workspace, activate an eligible plan or trial and publish a reviewed draft.
2. Configure appearance, public profiles, reader features and a custom subdomain or /blog address.
3. Use workspace credentials from a server to retrieve published blog content with the Enterprise read-only API.

## Motivation
Publish an organizational blog without building a separate publishing system. Keep subscriptions, credits, content and permissions scoped to the active workspace.

## Source and assumptions
Migrated from the application’s /docs page and checked against truhuddle/src/lib/developer-api.ts, plans.ts, billing-plans.ts and domain-connection.ts on 2026-10-30. The intended external docs hostname is docs.truhuddle.com; connecting that hostname in Mintlify and DNS is still required.
