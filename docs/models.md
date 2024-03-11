# Models

This models document explains the models folder in each table file and what is in that table

## Contents

- [User](#user)
- [Biodata](#biodata)
- [Admin](#admin)
- [Background](#background)
- [VisionMision](#visionmision)
- [LeadershipStructure](#leadershipstructure)
- [Devision](#devision)
- [Project](#project)
- [Cooperation](#cooperation)
- [Gallery](#gallery)
- [AboutUs](#aboutus)

## User

Mention every `attribute`, `guarded`, `hidden`, and any `methods` available to the user

#### Attibute:

- id
- email
- password
- role
- remember_token
- status

#### Guarded:

- id
- remember_token
- status

#### Hidden:

- password
- remember_token

#### Methods

- `someBiodata(): belongTo`

## Biodata

#### Attibute:

- nim
- name
- study_program
- devision
- semester
- address
- phone
- photo
- user (relation N-N users table)

#### Methods

- `user(): hasMany`

## Admin

- id
- email
- password
- phone
- remember_token

#### guarded

- id
- remember_token

## Background

#### Attiribute:

- id
- content

#### Guarded

- id

#### Methods

- `admin(): belongsTo`

## VisionMision

#### Attribute:

- id
- content

#### Guarded:

- id

#### Methods

- `admin(): belongsTo`

## LeadershipStructure

#### Attribute:

- id
- content
- image?

#### Guarded:

- id

#### Methods

- `admin(): belongsTo`

## Devision

#### Attribute:

- id
- name
- content

#### Guarded:

- id

#### Methods

- `admin(): belongsTo`

## Project

#### Attribute:

- id
- image?
- title
- description
- type `('UKM', 'DEVISION')`

#### Guarded:

- id
- type

#### Methods

- `admin(): belongsTo`

## Cooperation

#### Attribute:

- id
- image
- content

#### Guarded:

- id

#### Methods

- `admin(): belongsTo`

## Gallery

#### Attribute:

- id
- photo

#### Guarded:

- id

#### Methods

- `admin(): belongsTo`

## AboutUs

#### Attribute:

- id
- content

#### Guarded:

- id

#### Methods

- `admin(): belongsTo`
