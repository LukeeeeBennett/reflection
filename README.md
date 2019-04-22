# @lbennett/reflection

> Copy files from external storage to internal storage, then move them back and trash when you're done.
>
## Installation

```
npm install --global @lbennett/reflection
# OR
yarn global add @lbennett/reflection
```

Uses a `trash` command instead of `rm` to delete local files/directories. _I would like to change this._

`brew install trash` - http://hasseg.org/trash/

## Usage

1\. Set environment variables for external and internal storage locations.

```
REFLECTION_EXTERNAL_STORAGE_LOCATION="/Volumes/external/reflection-workspace"
REFLECTION_INTERNAL_STORAGE_LOCATION="/Users/me/reflection-workspace"
```

2\. Execute commands

`reflection summon useless-project`
* copy directory `useless-project` from external location to internal location

`reflection banish useless-project`
* copy directory `useless-project` from internal location to external location and
trash the internal version
