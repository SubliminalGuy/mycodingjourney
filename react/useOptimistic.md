#### What does the **useOptimistic** hook do?

The **useOptimistic** hook temporarily updates states that have been changed (e.g. via a Form Submit) **before** the state changes have been asynchronously processed. If the underlying change request changes the state bounces back to its prior value(s). **useOptimistic** improves the perceived performance of the UI.