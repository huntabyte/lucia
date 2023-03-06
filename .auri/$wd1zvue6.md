---
package: "lucia-auth" # package name
type: "minor" # "major", "minor", "patch"
---

**Breaking changes** Better integrate single use keys and clean up API
    - Only persistent keys can hold passwords
    - Update `Key` type
    - Deprecate `getKeyUser()`
    - Replace `validateKeyPassword()` with `useKey()`
    - Replace `data.key` with `data.primaryKey` for `createUser()`
    - Update `createKey()`
    - `getAllUserKeys()` returns all keys, including those expired