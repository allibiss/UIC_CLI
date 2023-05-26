# Dialogue design: Command Line User Interface (CLI) for Conversational User Interface
## Introduction
The intended goal of this user interface is to allow users to apply for an ID card via their mobile phone in an immediate and quick manner. This will enable them to avoid physically traveling to government services, which usually requires great investment of both time and money.

The main challenge addressed by this CLI is to provide a fast and immediate service with concise prompts, allowing users to have their physical ID card delivered to their homes or generate a digital version on their mobile phones. The primary hurdle is confirming the user's identity, which is typically done in person. To overcome this issue, the CLI will incorporate the option of an official online meeting to perform the necessary identity verification procedures.

Key considerations for implementing the user interface include:
- Ensuring ease of use for users with limited technological experience
- Minimizing the number of questions asked during the application process
- Guaranteeing secure processing of personal data
- Clearly communicating the required procedures to the users
- Enabling online meetings for identity confirmation, avoiding the need to visit physical offices
- Offering the option to receive the ID card by mail at the user's specified address
- Providing a digital version of the ID card for users to store on their mobile phones

##
To understand the user's journey, here is an example of the cognitive walkthrough for the main user-related tasks within the CLI:
1. Log on to the service
2. Wait for the service to launch
3. Answer questions regarding personal information
4. Enter personal photograph retrieval code
5. Enter an identification (banking ID, certificate card, mobile ID)
6. Wait for the information to be processed
7. Confirm participation in the eventual official online recognition meeting
8. Choose a digital ID card or for it to be sent
9. If choosing to have it sent, confirm shipping address
10. Pay for the ID card
11. Wait for confirmation of payment and successful completion of the service
12. Exit the service

Upon completion, the user will receive a notification regarding any online appointment and confirmation of the successful creation of their ID card.

## Guidelines that led to the implementation
The implementation of this CLI follows several guidelines to ensure a user-friendly and efficient experience, particularly for users with limited technological capabilities. These guidelines are as follows:
1. Menu Selection: The dialogue structure begins with a menu selection approach, minimizing the need for user training. Menu selection provides clear options, streamlines decision-making, and facilitates error handling. It also accommodates occasional users and reduces the learning curve and keystrokes.
2. Question and Answer Dialogue: In addition to menu selection, the CLI incorporates a question and answer dialogue to guide users through input requirements. This approach requires minimal user training and offers precise directions for user input. While power users may experience slightly slower interactions, the advantages outweigh the disadvantages, considering sporadic usage and less tech-savvy users.
3. Goal-based Finite-state Dialogue: The dialogue structure follows a goal-based approach with finite-state characteristics. The system initiates and controls the conversation flow, asking simple questions and expecting straightforward, individual answers. "Slots" with known structures and parameters are utilized to enhance conversation and expedite the process, benefiting power users. Clear instructions accompany the slots to facilitate accurate user input.
4. Simple and Unambiguous Feedback: After each user action, the system provides simple, clear, and unambiguous feedback. This feedback aims to prevent misunderstandings, bridge the gap of evaluation in terms of system perception and feedback, and adhere to the principles of good design. The system consistently invites the user to proceed with the next action, ensuring a smooth interaction.
5. Presentation of User Alternatives: To optimize the effectiveness, efficiency, and satisfaction of the interaction, the CLI always presents available user alternatives. For example, if a user does not wish to perform any action within the menu, they can easily exit the session. The CLI's conceptual model mirrors an order process, guiding users through introduction, information input, and confirmation stages. Clear relationships between stages are presented to enhance user comprehension.

Considering the target user group's lack of confidence with technology, this highly structured dialogue approach, which requires input from the user and provides output after each action, proves to be the most suitable method for realizing this CLI. Minimal user skills are required, as the interaction can be likened to any daily offline order experience. The command line interface uses straightforward terms and employs a basic and friendly dialogue to encourage user adoption of the technology.
