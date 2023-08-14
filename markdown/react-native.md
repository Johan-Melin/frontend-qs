**[⬆ Back to Contents](/README.md)**

## React Native

1. <details><summary>How many threads run in React Native?</summary>

   React Native runs a single UI thread and multiple native threads.

   **UI Thread**: React Native runs a single UI thread, also known as the "JS thread," which is responsible for handling JavaScript execution, UI updates, and event handling. This thread is where your React Native code runs, and it is crucial to keep this thread responsive to ensure a smooth user experience.

   **Native Threads**: React Native communicates with the native platform through bridge modules. When you call a native module from JavaScript, the bridge transfers the request to a separate native thread, where the corresponding native code is executed. This architecture allows React Native to take advantage of the native platform capabilities while keeping the UI thread free from blocking operations.

   It's important to note that the number of native threads can vary depending on the platform and the number of active bridge modules. The UI thread is the most critical thread, and it's essential to avoid blocking it with time-consuming operations to maintain responsiveness in your React Native application. Always use asynchronous and non-blocking code where possible, and consider using background threads for heavy computations or long-running tasks to prevent UI freezing.
   </details>

**[⬆ Back to Contents](/README.md)**
