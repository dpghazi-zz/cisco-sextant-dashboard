# Cisco Sextant App 
![Kapture 2022-08-17 at 23 52 03](https://user-images.githubusercontent.com/94224903/185320508-94563001-9d60-4c9a-a2b5-9687e8b08bcb.gif)
Note: Using VPN to hide personal IP address ¯\_(ツ)_/¯
## **Project Description**
- The Sextant Networking Dashboard is a single-page application meant to assist field technicians with their day-to-day tasks. 
- This web application uses React for the frontend to display the user’s public IP addresses (both ipv4 and ipv6) and the packet latency associated with a service called Pylon. 
- The user's public IP addresses are fetched from the <a href="https://www.ipify.org/" target="_blank">ipify API</a> and the packet latency can be streamed using WebSocket connections.

### **Overview**

- Task 1: Project Initialization
  - Initialized a new react app using the node package manager (npm).
- Task 2: Design the Sextant Frontend
  - Created a banner component at the top of the page which displays the site’s title.
  - Created an exhibit component that displays a heading.
  - Created child components which wrap the components to logically separate different data points.
- Task 3: Display the User's Public IP
  - Created a new component to collect and display the user’s public IP addresses.
    - The component makes an HTTP request to the ipify API as soon as it is mounted and surface the resultant data to the user.
    - The component accepts a prop that determines whether it requests an ipv4 address or an ipv6 address.
  - Added two instances of this component to the page, both wrapped in an exhibit component from the last task.
    - One displays the user’s ipv4 address, and the other displays the user’s ipv6 address.
- Task 4: Stream Data from a Networked Service
  - Created a new React Component, which displays packet latency from Pylon.
  - Added the component to my React app, living inside an Exhibit.

### Language **& Tools**

- JavaScript (React.js)
- HTML/CSS
- ipify API
- WebSocket
- Pylon
