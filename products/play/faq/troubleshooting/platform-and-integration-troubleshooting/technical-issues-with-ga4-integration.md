# Technical Issues with GA4 Integration

## Overview
Nudestix encountered a specific issue while integrating Google Analytics 4 (GA4) with Tolstoy. The problem arose because Tolstoy events were being sent directly to GA4, bypassing Google Tag Manager (GTM). This direct transmission conflicted with Nudestix's Consent Management Platform (CMP) setup.

## Details
### Direct Event Transmission
Tolstoy events were not routed through GTM as expected. Instead, they were sent straight to GA4. This direct approach can be problematic for organizations that rely on GTM for managing and controlling their analytics and marketing tags.

### Conflict with CMP
Nudestix's CMP setup was designed to work with GTM. The direct sending of events to GA4 bypassed the CMP, leading to potential compliance and data management issues. CMPs are crucial for ensuring that user consent is properly managed and that data collection complies with privacy regulations.

## Conclusion
The issue faced by Nudestix highlights the importance of ensuring that all analytics events are properly routed through GTM, especially when a CMP is in place. This ensures that user consent is respected and that data collection processes remain compliant with relevant regulations.