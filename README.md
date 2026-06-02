# Notes
Tutorial notes for Software Testing

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/56284a7b-4daf-4ca9-91fd-f1038b57a502" />

<img width="622" height="572" alt="image" src="https://github.com/user-attachments/assets/2f24fb9a-31aa-4c3a-bc7f-e90638ad53ff" />


---

- Unit testing involves isolating units so that functionality can be confirmed before units are integrated with other parts of the application

<img width="1000" height="470" alt="image" src="https://github.com/user-attachments/assets/b3f21764-c2e0-4947-8401-d6c55cd33d05" />

---

- Start with the system model.
- The system model contains the System Under Test (SUT).
- The SUT does not exist in isolation; it interacts with other objects in the system model that are not yet implemented. These objects are called collaborators.
- Since the real collaborators may not be available or implemented, additional objects are introduced into the test model. These substitute objects are called test doubles.
- Use test doubles during testing.
- Test doubles act as stand-ins for the collaborators, allowing the SUT to be tested independently of its actual dependencies.

<img width="816" height="337" alt="image" src="https://github.com/user-attachments/assets/bdff8471-bec6-4cc1-b81a-ea2421d44b90" />

---

- Dummy: Objects passed around but never actually used. They serve merely to fill parameter lists and avoid null reference errors during setup.
- Fake: Lightweight, working implementations of the component. They mimic the behavior of the real thing but take shortcuts that make them suitable for testing rather than production (e.g., an in-memory database instead of a full PostgreSQL cluster).
- Stub: Objects that provide canned, hardcoded answers to calls made during the test. They do not respond to anything outside what is explicitly programmed for the scenario and don't care how they are called.
- Mock: Objects pre-programmed with expectations. They verify that the system under test (SUT) calls them correctly, throwing an error if expected calls are missed or if unexpected calls are made.
- Spy: Objects that wrap a real object but also record indirect outputs (such as arguments passed to them) for later verification. This allows you to test real behavior while also tracking the interactions.

<img width="522" height="325" alt="image" src="https://github.com/user-attachments/assets/8f7c6aef-6697-4ec1-8f16-c411dbcebdc0" />


