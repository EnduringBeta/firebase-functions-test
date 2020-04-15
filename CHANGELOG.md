- `wrap` method now accepts `resource` as override in Context object, example:

  ```
  const wrapped = test.wrap(require("../src/index").myFirestoreFunction);
  wrapped(data, {
    resource: {
      name: ""projects/my-project/databases/(default)/documents/users/user-123",
    },
  });
  ```
  