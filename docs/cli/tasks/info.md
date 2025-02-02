## `mise tasks info [OPTIONS] <TASK>` <Badge type="warning" text="experimental" />

```text
[experimental] Get information about a task

Usage: tasks info [OPTIONS] <TASK>

Arguments:
  <TASK>
          Name of the task to get information about

Options:
  -J, --json
          Output in JSON format

Examples:

    $ mise tasks info
    Name: test
    Aliases: t
    Description: Test the application
    Source: ~/src/myproj/mise.toml

    $ mise tasks info test --json
    {
      "name": "test",
      "aliases": "t",
      "description": "Test the application",
      "source": "~/src/myproj/mise.toml",
      "depends": [],
      "env": {},
      "dir": null,
      "hide": false,
      "raw": false,
      "sources": [],
      "outputs": [],
      "run": [
        "echo \"testing!\""
      ],
      "file": null,
      "usage_spec": {}
    }
```
