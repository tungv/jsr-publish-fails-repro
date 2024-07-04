## Reproduction steps

```
npx jsr publish
```

Expected
```
Checking for slow types in the public API...
Publishing @jerni/publish-test@0.0.4 ...
Successfully published @jerni/publish-test@0.0.4
Visit https://jsr.io/@jerni/publish-test@0.0.4 for details

Completed in 3s
```

Actual
```
Downloading JSR binary...
[00:00] [################################################>-] 37.5 MiB/38.3 MiB
Checking for slow types in the public API...
Publishing @jerni/publish-test@0.0.3 ...
error: Failed to publish @jerni/publish-test@0.0.3

Caused by:
    Failed to publish @jerni/publish-test at 0.0.3: failed to build module graph: Module not found "file:///src/lodash".
        at file:///src/index.ts:1:15
Child process exited with: 1
```

