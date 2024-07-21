**Vimeo-Event-Wall**

A simple web application for clients to preview multiple, concurrent Vimeo streams on an external display, supporting real-time management of up to n streams.

**User story:**
As a live producer, I want to preview multiple Vimeo streams simultaneously on an external display, so that I can effectively monitor and manage these live streams in real-time, ensuring smooth production and enabling timely interventions when needed.

**Context:**
Setting up a robust system for simultaneously previewing multiple live streams involves careful planning of both hardware and network infrastructure to handle high bandwidth and processing demands. This pattern provides a simpler alternative by leveraging Vimeo's embedding API to display multiple streams in a web application optimized for low latency and high performance.

Currently, Vimeo clients typically can stream up to three events simultaneously, each up to 12 hours in length (soon 24 for VE clients). For more than three concurrent streams, contractual arrangements with Vimeo are necessary. Considerations should include both upstream and downstream data consumption, implementation of eCDN for efficient network usage, and potential DVR options and security measures.

This project aims to create a web application that allows clients to preview multiple Vimeo streams simultaneously on an external display. The current requirement is to support the preview of n Vimeo streams, facilitating real-time management and oversight of these live streams by an external team.

**Approach:**
This is a rapid prototype implementation of the Vimeo API in HTML, accommodating multiple streams displayed within an array, simulating a broadcast monitoring video wall. The code sets up a web page with a 3x3 grid layout displaying Vimeo videos. Each video is embedded in an iframe within a styled container to maintain a consistent aspect ratio. The Vimeo Player API is used to control video quality and handle events like playback and quality changes.

**UML Deployment Diagram:**
![image](https://github.com/user-attachments/assets/07f7f5d6-ddc6-4ed6-825d-f9922686325a)

