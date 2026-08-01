# Portfolio-RToS
# Avionics RTOS — FreeRTOS Task Architecture

Runway-lighting and stall-warning avionics system demonstrating FreeRTOS
inter-task communication (FIFO queues) and priority-inversion protection
(mutex-based priority inheritance) on the ESP32-S3.

## Links
- 🔧 Wokwi simulation: [Live simulation](https://wokwi.com/projects/465314244970953729)
- 🎥 Demo video: [Watch on YouTube](https://youtu.be/MMff_ldJhpQ?si=nSrrUGV-I_qx0yJH)
- 📄 Project overview: [View PDF](https://drive.google.com/file/d/1-fqB-Qf8PrhsIJRd9cb0C6Lb8XBPZnjU/view?usp=drive_link)
- 📊 System architecture & WCET/RMS analysis: [View PDF]([https://drive.google.com/drive/folders/1m356GRnEJb1Amogcf...](https://drive.google.com/drive/folders/1m356GRnEJb1AmogcfUnNLZGdE5bDWZjR?usp=drive_link))


## Architecture
Two task clusters: an ITC cluster (queues) and a priority-inheritance
cluster (mutex), connected by a dedicated emergency-override path.
See the architecture PDF for full diagrams and analysis.
