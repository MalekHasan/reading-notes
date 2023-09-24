# React Native

## getting started with react native

- Name three Core Components of React Native and describe what they do.

1. ```<View>```	: A container that supports layout with flexbox, style, some touch handling, and accessibility controls.
2. ```<Text>```: Displays, styles, and nests strings of text and even handles touch events
3. ```<Image>```: Displays different types of images.

- What problem does React Native solve (why call it native)?

***React Native is an open source framework for building Android and iOS applications using React and the app platform’s native capabilities. With React Native, you use JavaScript to access your platform’s APIs as well as to describe the appearance and behavior of your UI using React components: bundles of reusable, nestable code.***

- What are the building blocks of a React Native app? How does that compare to a React app?

***the building block of a React Native app is ```Native Components```.React and React Native share some common concepts, React Native is tailored for building mobile applications and leverages native components and modules, while React is designed for web applications and interacts with the browser's DOM. However, both frameworks emphasize component-based development and the use of JSX to define UI elements.***

## expo

- What solution does expo provide?

***Expo aims to streamline the React Native development process by providing a complete development environment, a wide range of pre-built functionality, and simplified deployment options, all of which are designed to make it easier for developers to create high-quality mobile apps.***

- Expo tries to manage as much of the complexity of building apps as possible, which is why we call it the ____ workflow.

***Managed***

- What is the difference between React Native and Expo?

***React Native CLI apps require macOS in order to build iOS apps – meaning Windows users cannot develop iOS apps without some sketchy workarounds. Expo completely bypasses this limitation by offering a hosted service called EAS Build for building app binaries for your Expo and React Native projects.***

## expo snack

- Checkout this tool. What does snack allow you to do?

***Snack is a convenient online development environment for React Native that simplifies the process of writing, testing, and sharing React Native code. It's particularly useful for quick prototyping, learning React Native, collaborating with others, or sharing code examples with the community.***

## ejecting

- What does “eject” mean within the context of Expo?

***The term "eject" was popularized by create-react-app, and it is used in Expo to describe leaving the cozy comfort of the standard Expo development environment, where you do not have to deal with build configuration or native code.***

- When should you not eject?

1. When You Prefer a Streamlined Development Experience.
2. When You Don't Need Access to Specific Native Modules.
3. When You Want to Focus on JavaScript Development.
4. When You Want to Rapidly Prototype and Iterate.
5. When You Don't Want to Deal with Build and Configuration Tasks.
6. When You Don't Need Advanced Customization.

- Why might you choose to eject?

***you would choose to eject from Expo when your project's requirements demand greater control, customization, or access to native code and native modules. Ejecting provides the flexibility needed to meet these specific development needs, but it also comes with increased complexity and responsibility for managing native code and configurations. Therefore, the decision to eject should be carefully considered based on your project's unique requirements.***