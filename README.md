# Cisco Sextant Dashboard App
## **Project Description**
- The Sextant Networking Dashboard is a single-page application meant to assist field technicians with their day-to-day tasks. 
- This web application uses <a href="https://github.com/facebook/create-react-app" target="_blank">React</a> for the frontend to display the user’s public IP addresses (both ipv4 and ipv6) and the packet latency associated with a service called <a href="https://www.npmjs.com/package/pylon" target="_blank">Pylon</a>. 
- The user's public IP addresses are fetched from the <a href="https://www.ipify.org/" target="_blank">ipify API</a> and the packet latency can be streamed using <a href="https://www.npmjs.com/package/websocket" target="_blank">WebSocket connections</a>.

### **Overview**

- **Initializing Project**
  - Initialized a new react app using the node package manager (npm).
- **Designing the Sextant Frontend**
  - Created a banner component at the top of the page which displays the site’s title.
  - Created an exhibit component that displays a heading.
  - Created child components which wrap the components to logically separate different data points.
- **Displaying the User's Public IP**
  - Created a new component to collect and display the user’s public IP addresses.
    - The component makes an HTTP request to the ipify API as soon as it is mounted and surface the resultant data to the user.
    - The component accepts a prop that determines whether it requests an ipv4 address or an ipv6 address.
  - Added two instances of this component to the page, both wrapped in an exhibit component from the last task.
    - One displays the user’s ipv4 address, and the other displays the user’s ipv6 address.
- **Streaming Data from a Networked Service**
  - Created a new React Component, which displays packet latency from Pylon.
  - Added the component to my React app, living inside an Exhibit.

## Result
![Kapture 2022-08-26 at 16 54 25](https://user-images.githubusercontent.com/94224903/187005244-ada3ab46-3745-40b3-88fd-c025f149af59.gif)


### Language **& Tools**

- JavaScript (React.js)
- HTML/CSS
- ipify API
- WebSockets Protocol
- Pylon
