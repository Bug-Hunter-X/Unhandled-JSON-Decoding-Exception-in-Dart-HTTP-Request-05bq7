# Unhandled JSON Decoding Exception in Dart

This repository demonstrates a common error in Dart when handling HTTP requests and JSON decoding. The `bug.dart` file shows the code with the error, while `bugSolution.dart` provides the corrected version.

The issue arises from the lack of explicit error handling during `jsonDecode`.  If the API returns invalid JSON, the application will crash. The solution adds a `try-catch` block around `jsonDecode` to gracefully handle parsing errors.