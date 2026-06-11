# Database Schema - QuickApply AI

## Overview

The QuickApply AI database is designed to store user information, profile details, uploaded documents, and application records. The system consists of four main entities: User, Profile, Documents, and Applications.

---

## User Table

| Field Name | Data Type |
| ---------- | --------- |
| user_id    | Long      |
| name       | String    |
| email      | String    |
| password   | String    |

---

## Profile Table

| Field Name    | Data Type |
| ------------- | --------- |
| profile_id    | Long      |
| user_id       | Long      |
| dob           | Date      |
| gender        | String    |
| mobile        | String    |
| address       | String    |
| qualification | String    |

---

## Documents Table

| Field Name  | Data Type |
| ----------- | --------- |
| document_id | Long      |
| user_id     | Long      |
| photo       | String    |
| signature   | String    |
| resume      | String    |

---

## Applications Table

| Field Name     | Data Type |
| -------------- | --------- |
| application_id | Long      |
| user_id        | Long      |
| form_name      | String    |
| status         | String    |
| applied_date   | Date      |

---

## Relationships

* One User can have one Profile.
* One User can upload multiple Documents.
* One User can submit multiple Applications.
* Applications are linked to the corresponding User account.
