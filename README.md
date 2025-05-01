# Digital-Rescue-Station

This tool helps rescue content from obsolete digital formats, such as ZIP disks or CDs, preserving their structure and making files accessible and searchable online.

Digital Rescue Station - Accessibility Strategy

Overview:
This document outlines the accessibility features and standards compliance of the "Digital Rescue Station" proof of concept, designed to demonstrate best practices in digital preservation and inclusive access.

Accessibility Features:

1. Visual Accessibility:
- High-contrast themes with toggle support (light/dark mode).
- Resizable text via font-size slider or keyboard shortcuts.
- Legible sans-serif fonts (e.g., Arial, Open Sans); no italics or all caps.
- Alt-text for all non-text elements such as icons and previews.
- Colorblind-safe palettes avoiding color-only communication.

2. Keyboard Navigation:
- All elements are navigable via keyboard (Tab, Enter, Arrow keys).
- Keyboard shortcuts for key functions like upload, convert, and download.

3. Screen Reader Support:
- Semantic labels for all UI elements.
- ARIA labels for custom components.
- Action descriptions written clearly and precisely.

4. Cognitive Accessibility:
- Step-by-step plain language instructions.
- Icons paired with text labels for clarity.
- Option to download a transcript or action log.

5. Hearing Impairment:
- Visual alerts for all notifications and system messages.
- Text explanations provided for any multimedia content.

Streamlit Implementation Tips:

| Feature                    | Streamlit Implementation Suggestion                        |
|---------------------------|------------------------------------------------------------|
| High contrast toggle       | st.toggle("High Contrast Mode") + custom CSS              |
| Font size slider           | st.slider("Font Size", min_value=12, max_value=24)        |
| Keyboard-friendly buttons  | Streamlit buttons are tab-navigable by default            |
| Screen reader compatibility| Use st.markdown with semantic structuring                 |
| Accessible file upload     | st.file_uploader("Upload a file", label_visibility="visible") |
| Text-to-speech preview     | Optional with pyttsx3 (desktop) or browser TTS integration |

Accessibility Customization Options:
Include a "Customize My View" panel allowing users to:
- Toggle contrast or theme
- Resize text
- Enable simplified (reduced-clutter) view
- Activate screen-reader optimization mode

Compliance and Best Practices:
This accessibility strategy aligns with WCAG 2.1 guidelines and adheres to archival best practices that prioritize inclusive access to cultural memory institutions. The approach also supports the New Brunswick Government’s commitment to equity and universal design.


