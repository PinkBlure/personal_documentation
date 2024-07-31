# How to start a Rails project

For creating a new Rails project, use the next command.

```bash
rails new project_name
```

To use Postgresql within the project, use the next command. By default, Rails use Sqlite. Updating to Postgresql instead gives us the possibility to escalate the project later on.

```bash
rails new project_name -d postgresql
```