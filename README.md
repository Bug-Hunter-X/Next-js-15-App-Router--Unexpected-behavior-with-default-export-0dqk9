# Next.js 15 App Router: Unexpected Behavior with Default Export in Page Component

This repository demonstrates an unexpected behavior in Next.js 15's App Router when using a default export in a page component.  The issue involves the rendering of the page component and potential inconsistencies. 

## Bug Description

When a page component uses a default export, it might not render as expected in the app directory, leading to blank pages or other unexpected behavior. This seems to be related to how the App Router handles default exports versus named exports in the new architecture. 

## How to Reproduce

1. Clone this repository.
2. Run `npm install`.
3. Run `npm run dev`.
4. Observe that the page renders unexpectedly (blank page, errors). 

## Solution

The solution involves changing the default export to a named export. This aligns with how the App Router seems to be designed to work most reliably with page components.