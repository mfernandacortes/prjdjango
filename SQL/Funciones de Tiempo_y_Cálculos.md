# Funciones de Tiempo y Cálculos en MySQL

## Obtener fecha y hora actual

```sql
SELECT NOW();
SELECT CURRENT_TIMESTAMP();
```

---

## Operaciones con horas

### Agregar 15 minutos a una hora

```sql
SELECT ADDTIME('09:45:00', '00:15:00');
```

### Restar 15 minutos a una hora

```sql
SELECT SUBTIME('09:45:00', '00:15:00');
```

---

# Cálculos con fechas

## Obtener fecha actual

```sql
SELECT CURDATE();
```

---

## Sumar días a una fecha

```sql
SELECT ADDDATE(CURDATE(), INTERVAL 15 DAY);
```

---

## Restar días a una fecha

```sql
SELECT SUBDATE(CURDATE(), INTERVAL 15 DAY);
```