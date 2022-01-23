# Octo Reminder

[https://github.com/apps/octo-reminder](https://github.com/apps/octo-reminder)

## Support
Having troubles with [Octo Reminder](https://github.com/apps/octo-reminder)? Open a new issue [here](https://github.com/set-reminder/issues/issues/new).

## Installation

1. [Install Octo Reminder](https://github.com/apps/octo-reminder/installations/new)
2. Set up your language and timzone in the configuration (see below for details).

## Configuration
You can set up your configuration either globally or per repository.

### Global
1. Create a `.github` repository (private or public)
2. In this repository, create a new file: `.github/octo-reminder.yml`

### Per Repository
Just create a new file `.github/octo-reminder.yml` in the repository where you want to apply your configuration. 
This file **will override your global configuration**.

###  octo-reminder.yml
```yml
# Octo Reminder Configuration

## Command Prefix
### Define the prefix of your custom command.
### Type: '/' | '!'
### Default: '@' (works only in combination with command_name 'set-reminder')
command_prefix: '@'

## Command Name
### Define the name of your custom command.
### Type: String
### Default: 'set-reminder'
command_name: 'set-reminder'

## Language
### Define the language.
### Type: 'en' | 'fr' | 'de' | 'pt' | 'nl' | 'ja'
### Default: 'en'
language: 'en'

## Timezone
### Define the timezone.
### Type: String (see also https://github.com/moment/moment-timezone/blob/develop/data/packed/latest.json)
### Default: 'Europe/London'
timezone: 'Europe/London'

## Default Hour
### Define the hour that will be used, when no time is specified.
### Type: Number
default_hour: 0

## Default Minute
### Define the minute that will be used, when no time is specified.
### Type: Number
default_minute: 0
```

## Usage
```
@set-reminder [date] [message]
```
Examples:

<img width="621" alt="Octo Reminder Usage" src="https://user-images.githubusercontent.com/15997450/150693285-81ecec47-ca1f-4ba5-9d57-a93e8e8535ed.png">

