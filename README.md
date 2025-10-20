# Phanes

A browser-side analytics toolkit for online forms & polls

![Phanes Logo](./logo.svg)

## Description

A web app for tracking impressions, drop-offs and user behaviour in surveys/forms — designed for online polls and internal research flows, with click/hover/scroll heatmaps and privacy-first client-side aggregation.

## Features

- **Interactive Heatmaps**: Visualize where users click, scroll, and hover within online forms and polls, identifying areas of high engagement and potential friction.
- **User Behavior Funnels**: Track user progression through forms to pinpoint drop-off points and optimize the flow for better completion rates.
- **Client-Side Data Aggregation**: Utilize techniques like HyperLogLog (HLL) and HyperMinHash to aggregate data directly in the user's browser, preserving privacy and reducing server load.
- **Fully Homomorphic Encryption (FHE)**: Implement FHE to perform computations on encrypted data without exposing it, ensuring confidentiality and compliance with data protection regulations.
- **Adaptive User Profiling**: Automatically segment users based on their interaction patterns, such as response times and consistency, to tailor the user experience and identify potential issues.
- **Behavioral Anomaly Detection**: Analyze response intervals and patterns to detect inconsistencies or potential fraudulent activity, enhancing the reliability of collected data.
- **Persona-Based Interaction Simulation**: Create visual simulations representing different user personas to understand diverse interaction styles and inform design decisions.
- **Dynamic Feedback Loops**: Incorporate real-time feedback mechanisms to adjust questions or prompts based on user responses, improving engagement and data quality.
- **Accessibility and Inclusivity Features**: Ensure the platform is accessible to users with disabilities by adhering to WCAG standards and offering multilingual support.
- **Customizable Analytics Dashboard**: Provide users with a personalized dashboard to view and analyze their data, offering insights into user behavior and form performance.
- **Direct Import of Existing Form Data**: Seamlessly upload form responses from CSV or XLSX files into Phanes, enabling the analysis of historical data without the need for re-entry.
- **Automated Data Integration**: Integrate Phanes with external platforms such as Google Sheets or Microsoft Excel to automatically pull and analyze form data in real-time, streamlining data workflows.

## Analysis ideas

- **Item Response Theory (IRT) Integration**: Implement IRT to model question difficulty and respondent ability, similar to Brazil's ENEM exam. This allows for dynamic assessment of question effectiveness and participant engagement.
- **Behavioral Friction Detection**: Utilize mouse movement patterns, such as hover duration and cursor path analysis, to identify areas where respondents experience difficulty or hesitation, indicating potential friction points in the form.
- **Anomaly and Dishonesty Detection**: Analyze response times and interaction patterns to flag suspicious behaviors, such as rapid answering or inconsistent responses, which may indicate dishonest or inattentive respondents.

### Persona-Based Labeling

Develop personas based on common user behaviors and assign labels accordingly:

- _O Cronista_: Thoughtful and detailed in responses.
- _O Político_: Strategic and possibly agenda-driven.
- _O Cético_: Questioning and analytical.
- _O Desatento_: Quick and possibly superficial in responses.

Utilize behavioral data to create segments that reflect user engagement levels and interaction styles:

- **Engaged Respondents**: Users who spend time reflecting on questions and provide comprehensive answers.
- **Strategic Participants**: Users who navigate through the form with specific objectives, possibly influenced by external factors.
- **Hesitant Users**: Users who take longer to answer, possibly indicating uncertainty or the need for more information.
- **Passive Respondents**: Users who quickly move through the form, potentially skipping questions or providing minimal input.

These segments can inform the design of the form, helping to identify areas that may cause friction or disengagement.

### Visual Simulation of User Personas

An interactive representation illustrating how different user profiles—such as O Cronista, O Político, O Cético, and O Desatento—engage with online forms, providing insights into their behaviors, hesitations, and navigation patterns.

- **Enhanced User Understanding**: Visualizing how distinct personas interact with forms helps identify specific needs, frustrations, and friction points, leading to a more empathetic design approach.
- **Informed Design Decisions**: By observing persona-specific behaviors, designers can tailor form layouts, question phrasing, and interaction flows to better align with user expectations and reduce drop-off rates.
- **Effective Stakeholder Communication**: Simulations serve as compelling tools to demonstrate user behaviors to stakeholders, facilitating discussions and aligning teams on user-centered design strategies.

### 🚀 Leveraging WebAssembly for Performance and Extensibility

#### ⚡ High-Performance Client-Side Analytics

By compiling analytics modules into WebAssembly (WASM), **Phanes** can execute complex data processing directly within the user's browser. This approach reduces server load, enhances responsiveness, and ensures that sensitive data remains private, as computations occur locally. For instance, integrating tools like DuckDB compiled to WASM allows for efficient SQL-based analytics without the need for server-side databases. :contentReference[oaicite:6]{index=6}

#### 🔌 Dynamic Plugin Architecture

**Phanes** can adopt a plugin-based architecture using WASM to support dynamic loading and execution of custom modules. This enables seamless extensibility, allowing developers to add new features or modify existing ones without altering the core application. Frameworks like Extism facilitate this by providing a lightweight environment for running WASM modules across various platforms. :contentReference[oaicite:14]{index=14}

#### 🧩 Custom Interfaces and Integration

To ensure smooth integration of custom WASM modules, **Phanes** can define clear interfaces and provide documentation for developers. This approach allows for the creation of tailored analytics tools, such as specialized heatmap generators or custom anomaly detection algorithms, which can be seamlessly incorporated into the **Phanes** ecosystem.

#### 🔐 Secure and Isolated Execution

WASM modules operate in a sandboxed environment, ensuring that custom code runs securely without compromising the integrity of the host application. This isolation prevents unauthorized access to sensitive data and system resources, making it safe to execute third-party modules within **Phanes**.

#### 🧠 Enhancing **Phanes** with WASM

Integrating WASM into **Phanes** not only boosts performance but also fosters a vibrant ecosystem of customizable analytics tools. By enabling high-performance, secure, and extensible client-side analytics, **Phanes** can offer a more dynamic and user-centric experience.

If you're interested in exploring how to implement WASM-based plugins or need assistance in setting up a WASM runtime within **Phanes**, feel free to ask!
