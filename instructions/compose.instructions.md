---
applyTo: '**/*.compose.yml'
---

- Add `name` property to the root with the project name
- Do not wrap the next properties in quotes unless they contain special characters
- Follow the next order of properties on the root level: 
  1. `volumes`
  2. `networks`
  3. `services`
- Follow the next order of properties on the service level:
  1. `image`
  2. `container_name`
  3. `build`
  4. `environment`
  5. `expose`
  6. `ports`
  7. `volumes`
  8. `networks`