# Configuración de Poetry

El repositorio ha sido configurado para usar **Poetry** como gestor de dependencias.

## Instalación inicial

Si aún no tienes Poetry instalado, instálalo con:

```bash
pip install poetry
```

## Instalar dependencias

```bash
poetry install
```

Esto instalará todas las dependencias especificadas en `pyproject.toml` y creará un ambiente virtual.

## Activar el ambiente virtual

```bash
poetry shell
```

O ejecutar comandos directamente con Poetry:

```bash
poetry run python app.py
```

## Agregar nuevas dependencias

```bash
poetry add nombre_paquete
```

Para dependencias de desarrollo:

```bash
poetry add --group dev nombre_paquete
```

## Actualizar `requirements.txt` desde Poetry

```bash
poetry export -f requirements.txt --output requirements.txt
```

## Verificar dependencias instaladas

```bash
poetry show
```

## Usar Streamlit con Poetry

```bash
poetry run streamlit run app.py
```
