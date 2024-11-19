# Laravel Todo App

## Despre Proiect 📋
Aplicație de management al sarcinilor dezvoltată în Laravel, implementând funcționalități CRUD, sistem de comentarii, categorii și etichete. Proiectul servește ca exemplu practic pentru gestionarea eficientă a task-urilor într-o echipă.

## Functionalități 🚀

✅ Gestionare completă a sarcinilor (CRUD)
📝 Sistem de comentarii pentru fiecare sarcină
🏷️ Categorii și etichete pentru organizare
🔄 Tranzacții pentru operațiuni complexe
💫 Interfață modernă și responsivă

## Tehnologii Utilizate 💻

- Laravel Framework
- MySQL
- Blade Templates
- CSS modern

## Structura Bazei de Date 🗄️
### Tabele și Relații
#### tasks
- id (primary key)
- title (string)
- description (text)
- category_id (foreign key)
- created_at (timestamp)
- updated_at (timestamp)

#### categories
- id (primary key)
- name (string)
- description (text)
- created_at (timestamp)
- updated_at (timestamp)

#### tags
- id (primary key)
- name (string)
- created_at (timestamp)
- updated_at (timestamp

#### task_tag (tabelă pivot)
- id (primary key)
- task_id (foreign key)
- tag_id (foreign key)
- created_at (timestamp)
- updated_at (timestamp)

#### comments
- id (primary key)
- content (text)
- task_id (foreign key)
- created_at (timestamp)
- updated_at (timestamp)

### Relații

Task -> Category: Many-to-One
Task -> Tags: Many-to-Many
Task -> Comments: One-to-Many
