# PurgeCSS removes dynamically generated Tailwind classes

This repository demonstrates a common issue with PurgeCSS and Tailwind CSS where classes added to the DOM dynamically after the initial build are removed by PurgeCSS. This can lead to unexpected styling issues. 

## Bug Description

The bug occurs when using dynamic content rendering in a framework like React or Vue.  If Tailwind CSS classes are added to elements after the initial page load, PurgeCSS, configured to optimize the CSS output, might mistakenly remove them. This leads to missing styles for the affected elements.

## Solution

The provided solution showcases how to address this problem by ensuring PurgeCSS is aware of the dynamically generated classes. This usually involves modifying the PurgeCSS configuration to include the dynamically generated content.
