# Entornos-7.2

Ejercicio 1 

``` mermaid
graph LR
    Usuario((Usuario))

    subgraph "Sistema de Luces"
        CU1([Encender Luces])
        CU2([Apagar Luces])
    end

    Usuario --- CU1
    Usuario --- CU2

```

```mermaid
graph LR
%% Definición de los Actores
Cliente((Cliente))
Administrador((Administrador))

subgraph "Sistema de Tienda Online"
%% Casos de Uso
CU1([Comprar Producto])
CU2([Aplicar Cupón Descuento])
CU3([Gestionar Stock])

%% Relación de Extensión (Opcional)
CU2 -.->|&lt;&lt;extend&gt;&gt;| CU1
end

%% Interacción de los actores
Cliente --- CU1
Administrador --- CU3
```


