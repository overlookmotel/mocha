This module is a fork of [mocha](https://www.npmjs.com/package/mocha) which makes just one small change.

In standard mocha, a tick is introduced in between running hooks (e.g. `beforeEach`) which are in a nested set of `describe` blocks. This makes it difficult to use mocha to test constructs like Promises where whether a tick has passed or not may be part of the subject under test. See [this issue](https://github.com/mochajs/mocha/issues/3009).

This module is identical to mocha except this additional tick is removed.
