# reflection

> Copy files from external storage to internal storage, then move them back and trash when you're done.

Uses `trash` to delete local files/directories because you shouldn't trust me.

`brew install trash` - http://hasseg.org/trash/

## usage

1\. Set environment variables for external and internal storage locations.

```
REFLECTION_EXTERNAL_STORAGE_LOCATION="/Volumes/external/reflection-workspace"
REFLECTION_INTERNAL_STORAGE_LOCATION="/Users/me/reflection-workspace"
```

2\. Execute

`./reflection summon useless-project`
* copy directory `useless-project` from external location to internal location

`./reflection banish useless-project`
* copy directory `useless-project` from internal location to external location and
trash the internal version
