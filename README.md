# Triton-Ultra-Zenitel-Connect-Pro-Webhook
Integration of Triton Ultra sensor with Zenitel Connect Pro via Webhook

This solution integrates a Zenitel Connect Pro with Triton Ultra sensors via Webhook running as a Node-red flow. Integration implements listening to live events for threats such as gunshots, glass break, keyword detection or air quailty. By using Node-red it's possible to add certain actions after the event is detected. This flow is used to issue a warning message which is stored on ZCP server, and place a call to operator after the event is detected and warning message is played.
To test this flow, follow next steps : 
1. Ensure that you have Triton Ultra subscription.
2. Ensure that events and actions are properly configured in Triton web interface.
3. Ensure the flow is deployed on Zenitel Connect Pro server, port 1880.
4. Ensure that nodes contain valid credentials and configuration.
5. Ensure that nodes contain valid directory numbers for playing warning messages.
6. Ensure that nodes contain valid directory numbers for establishing calls to the operator.
7. Use keyword such as "help" or use sample sound to simulate gunshot or noise or any other event you have configured prior.
8. Ensure that HTTP In node is properly configured in Node red and that it matches with HTTP configuration in Triton web interface .
9. Warning message should be played when the event is detected.
10. Call should be placed to the operator after the messsage is played.
11. Events are logged in Node-red debug window.

