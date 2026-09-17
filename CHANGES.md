# Todo App Changes

## What Was Done

The Todo app was updated to match the requested design:

- Added a full-page office background image.
- Added a centered, translucent white Todo panel with rounded corners.
- Styled the page with responsive spacing so it works on desktop and mobile screens.
- Added a centered `Todo App` heading.
- Added a larger todo input with an attached purple `+` button.
- Styled each task as a separate white row.
- Added orange edit buttons and red delete buttons.
- Added inline editing for existing tasks.
- Added the task counter at the bottom of the panel.
- Added the purple `Clear All` button.
- Added hover and focus states for buttons and inputs.
- Added a small panel entrance animation.

## Files Updated

### `static/style.css`

Contains the visual design, including:

- Background image and overlay
- Translucent panel
- Colors, spacing, borders, shadows, and typography
- Responsive layout rules
- Button hover effects
- Panel entrance animation

### `todo/templates/todo/list.html`

Contains the Todo interface and functionality, including:

- Add-task form
- Task list
- Edit form and edit button
- Delete button
- Task count
- Clear-all form
- JavaScript for showing inline edit fields

### `todo_project/settings.py`

Configured Django to find the project-level static files folder:

```python
STATIC_URL = 'static/'
STATICFILES_DIRS = [BASE_DIR / 'static']
```

## Verification

The database migrations were run successfully with:

```powershell
python manage.py migrate
```

Run Django checks from the folder that contains `manage.py`:

```powershell
cd todo_project
python manage.py check
```

Start the development server with:

```powershell
cd todo_project
python manage.py runserver
```

Then open `http://127.0.0.1:8000/` in the browser.
