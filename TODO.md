# TODO - ultrapro-email

## Bugs

- [ ] Cuenta "personal" falla en login IMAP (timeout 10s) - verificar App Password de Gmail

## Código

- [ ] Commit de cambios pendientes

## Documentación

(Sin tareas pendientes)

## Archivos modificados sin commit

- `mcp_email_server/emails/classic.py` - IMAPConnectionError, flags, cleanup debug
- `mcp_email_server/emails/models.py` - campos flags/keywords
- `mcp_email_server/app.py` - nuevos tools de flags
- `README.md` - documentación de flags
- `CHANGELOG.md` - features de flags
- `TODO.md` - actualizado

---

## Completado

### Documentación
- [x] README: documentar `check_unread`, `mark_as_read`, `mark_as_unread`
- [x] README: documentar auto-detección Markdown → HTML
- [x] README: documentar tamaños de email en respuestas
- [x] README: documentar elapsed time en respuestas
- [x] Crear CHANGELOG.md con historial de cambios

### Bugs
- [x] TimeoutError en login IMAP ahora muestra mensaje descriptivo (`IMAPConnectionError`)

### Código
- [x] Remover logging de debug en `get_flagged_emails`

### Documentación
- [x] README: documentar tools de flags (`list_flagged`, `set_flag`, `remove_flag`)
- [x] README: documentar `flags` y `keywords` en metadata de emails
- [x] CHANGELOG: agregar feature de flags/keywords

### Features
- [x] CRUDLEX Permissions por cuenta
- [x] `send_email` respuesta con sender + elapsed_ms
- [x] `check_unread` incluye tamaño de cada email
- [x] `list_emails_metadata` incluye tamaño de cada email
- [x] Campos `flags` y `keywords` en EmailMetadata y EmailBodyResponse
- [x] Tools: `list_flagged`, `set_flag`, `remove_flag`
- [x] Optimización: batch fetch de FLAGS en chunks de 50
