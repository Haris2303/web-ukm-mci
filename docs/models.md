# Models

This models document explains the models folder in each table file and what is in that table

## Contents

- [User](#user)
- [Biodata](#biodata)
- [Admin](#admin)

## User

Mention every `attribute`, `fillable`, `hidden`, and any `methods` available to the user

#### Attibute:

- id
- email
- password
- role
- remember_token
- status

#### Fillabel:

- email
- password
- role

#### Hidden:

- password
- remember_token

#### Methods

- `someBiodata(): belongTo;`

## Biodata

- nim
- name
- study_program
- devision
- semester
- address
- phone
- photo
- user (relation N-N users table)

## Admin

- id
- email
- password
- role
- remember_token
