# VidQL

**VidQL (Video Query Language)** is a domain-specific query and scripting language designed for **creative computing and media-aware systems**.

It enables developers to **query, manipulate, and automate structured data, media, and creative workflows** through a unified and expressive syntax.

---

## Vision

VidQL is part of **Video Artistic Technologies (VidArt)**, aiming to redefine how computers handle both **data and creativity**.

> Turning computers into creative instruments.

VidQL bridges the gap between:
- traditional data systems  
- and creative/media processing  

---

## Why VidQL?

General-purpose systems like PostgreSQL are powerful for structured data—but they are not designed for **creative or media-aware workflows**.

VidQL is built to:

- Handle **structured data and media together**
- Provide **intuitive syntax** for both querying and actions
- Enable **automation beyond traditional databases**
- Integrate deeply with creative and system-level tools

---

## Core Idea

VidQL is not just a query language.

It is a **query + action language**.

You don’t just *ask* for data—you can *act on it*.

---

## Features (Planned)

### Data + Media Support
- Structured data (tables, objects)
- Media-aware types:
  - `clip`
  - `timeline`
  - `frame`
  - `asset`

### Query System
- SQL-inspired syntax
- Filtering, grouping, transformations
- Time-based and metadata-based queries

### Action Layer
- Built-in operations:
  - `APPLY`
  - `TRANSFORM`
  - `PROCESS`
  - `RENDER`

### Automation
- Script workflows across data and media
- Batch operations and pipelines

### Extensibility
- Plugin system
- SDK support (Python, JavaScript)
- Custom data/media types

---

## Example Syntax

### Query structured data
```sql
SELECT users
WHERE active = true
