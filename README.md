**Vimeo-Event-Wall**

A simple web application enabling clients to preview multiple, concurrent Vimeo streams on an external display, supporting real-time management of up to n streams.

**User story:**
As a live producer, I want to preview multiple Vimeo streams simultaneously on an external display, so that I can effectively monitor and manage these live streams in real-time, ensuring smooth production and enabling timely interventions when needed.

**Context:**
Setting up a robust system for simultaneously previewing multiple live streams involves careful planning of both hardware and network infrastructure to handle high bandwidth and processing demands. This pattern provides a simpler alternative by leveraging Vimeo's API to display multiple streams in a web application optimized for low latency and high performance.

Currently, Vimeo clients typically can stream up to three events simultaneously, each up to 12 hours in length (soon 24 for VE clients). For more than three concurrent streams, contractual arrangements with Vimeo are necessary. Considerations should include both upstream and downstream data consumption, implementation of eCDN for efficient network usage, and potential DVR options and security measures.

This rapid prototype accommodates multiple streams displayed within an array, simulating a broadcast monitoring video wall and thus facilitating real-time management and oversight of these live streams by an external team.

**Implementation:**
The code sets up a web page with a 3x3 grid layout displaying 8 Vimeo live events. Each video is embedded in an iframe within a styled container to maintain a consistent aspect ratio. The Vimeo Player API is used to control video quality and handle events like playback and quality changes. eCDN is configured on Vimeo's backend.

**UML Deployment Diagram:**
![image](https://github.com/user-attachments/assets/07f7f5d6-ddc6-4ed6-825d-f9922686325a)



[![DOI](https://zenodo.org/badge/831154059.svg)](https://doi.org/10.5281/zenodo.15033373)



