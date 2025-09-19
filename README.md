Kindred: A Prototype for AI-Mediated Self-Architecture
Author: Anthony Perry Date: September 19, 2025 Project Status: Research Prototype
1. Abstract
Kindred is an interactive web-based prototype designed to explore the potential of Large Language Models (LLMs) as partners in the process of self-discovery and intentional living. The application guides users through a structured self-reflection process, capturing key facets of their identity and aspirations. This data is then used to generate a sophisticated, personalized "blueprint" prompt, enabling users to instantiate a tailored AI companion within existing generative AI platforms (e.g., Gemini, ChatGPT). This project serves as a proof-of-concept for AI-mediated self-architecture, investigating how technology can facilitate deeper self-awareness and personal alignment.
2. Theoretical Framework
This project is grounded in principles from Human-Computer Interaction (HCI), Affective Computing, and Narrative Psychology.
	•	Computational Self-Scaffolding: The core hypothesis is that an AI can act as a "scaffold" for self-reflection. By externalizing their thoughts and values into a structured format, users can gain a clearer perspective on their own inner world. The AI's role is not to provide answers, but to provide a framework that helps users construct their own meaning.
	•	Digital Phenomenology & The Astute Mirror: The application is designed to be an "Astute Mirror," reflecting the user's input back to them in a structured and illuminating way. This aligns with phenomenological approaches, focusing on the user's subjective experience. The AI companion, configured by the generated blueprint, is designed to perpetuate this mirroring process in subsequent interactions.
	•	Interactive Aesthetics: The user interface is a key part of the intervention. The dynamic, procedurally generated cloud background, which subtly responds to cursor movement, is designed to induce a state of calm and focus. This "affective computing" element aims to create an environment conducive to introspection, where the interface itself feels alive and responsive.
3. Technical Architecture & Implementation
Kindred is a client-side web application built with foundational web technologies, demonstrating proficiency in core programming without reliance on heavy frameworks.
	•	Frontend:
	◦	HTML5: Provides the semantic structure of the application.
	◦	CSS3: Used for styling, including custom properties (variables) for theming and a "glassmorphism" UI aesthetic.
	◦	JavaScript (ES6): Governs all application logic, including state management for the multi-step form, DOM manipulation, and API communication.
	•	Key Features:
	◦	Procedural Cloud Generation: The background is rendered on an HTML5 <canvas> element. It uses a Perlin noise algorithm to generate a fractal, cloud-like texture. The animation loop continuously updates the noise field and incorporates the user's cursor position as a "repulsion" force, creating an interactive "wind" effect.
	◦	Dynamic UI Rendering: The multi-step form is generated programmatically from a configuration object in the JavaScript. This makes the form easily extensible and maintainable.
	◦	Generative AI Integration: The application uses the fetch API to make a secure POST request to the Google Generative AI API. It sends a dynamically constructed prompt to generate a personalized welcome message for the user, demonstrating asynchronous programming and API interaction skills.
4. Ethical Considerations
As a project dealing with personal reflection, ethical considerations are paramount.
	•	Data Privacy: The application is entirely client-side. No user data is ever stored, transmitted to a server, or logged. The user's profile exists only in their local browser session and is cleared upon refresh.
	•	AI's Role and Limitations: The generated blueprint explicitly instructs the AI to state its limitations. It clearly defines itself as a tool for self-reflection, not a substitute for licensed therapists or medical professionals. This is a critical ethical guardrail to prevent misuse.
	•	Security Fortifications: The application implements a strict Content Security Policy (CSP) and Permissions-Policy via meta tags. This hardens the application against common web vulnerabilities like Cross-Site Scripting (XSS) and clickjacking, and follows the principle of least privilege by disabling unnecessary browser features.
5. Future Work & PhD Research Directions
This prototype serves as a launchpad for several potential avenues of academic research:
	•	Longitudinal Studies: A future version could incorporate secure, consent-based data storage (e.g., using Firebase with user authentication) to conduct longitudinal studies on how the user-Kindred relationship evolves over time. Research Question: How does long-term interaction with a personalized AI companion affect an individual's sense of self-clarity and goal alignment?
	•	Affective State Analysis: The user's text input within the application could be analyzed for sentiment and emotional tone. This data could be used to subtly adapt the UI (e.g., color palette) or the AI's initial welcome message to be more resonant with the user's current affective state.
	•	Comparative Analysis: A controlled study could compare the efficacy of this structured "blueprint" approach against unguided interaction with a generic chatbot for tasks related to personal goal setting and problem-solving.
6. Installation & Usage
	1	Clone the repository: git clone [https://github.com/](https://github.com/)[your-username]/kindred-ai.git
	2	
	3	
	4	Navigate to the directory: cd kindred-ai
	5	
	6	
	7	Open index.html: Open the index.html file in any modern web browser. As the project is fully client-side, no local server is required.
To use the application:
	1	Click "Begin" to start the self-reflection journey.
	2	Answer the series of questions to build your personal profile.
	3	Upon completion, the system will generate a welcome message and a detailed AI blueprint.
	4	Click the glowing orb to copy the blueprint to your clipboard.
	5	Follow the links to create a new "Gem" in Google Gemini or a new "GPT" in OpenAI, and paste the copied blueprint into the custom instructions field.
