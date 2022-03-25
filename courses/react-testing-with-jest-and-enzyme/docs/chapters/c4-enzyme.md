# Enzyme

## Que es Enzyme ?

Es una utilidad de testing de javascript que facilita el testeo de componentes de React.

[Web Oficial](https://enzymejs.github.io/enzyme/)

### Que es lo que Enzyme provee?
- Crea un `DOM Virtual` para testar.
- Permite el testeo sin necesidad de un navegador.
- Soporta el testeo aislado.
    - `Shadow Rendering`

### Diferencias entre Enzyme y React Testing Library
- Ambas librerias crean un `DOM Virtual`
- Diferencias filosoficas a la hora de hacer el testing.
- **Enzyme** soporta el testeo aislado.
- **React Testing Library** prefiere fuertemente el `testing funcional`.
    - Esto significa que interactua como un usuario lo haria.
    - Esto lo convierte en un test menos aislado.

### Por que elegir Enzyme?
- Porque prefieres un estilo de test mas tradicional:
    - El testing esta mas acoplado al codigo.
    - Los test unitarios son mas aislados.
    - Los tests son mas faciles de diagnosticar.
- Enzyme se adapta mejor para proyecto con código de prueba heredado (legacy test code).

### Por que elegir React Testing Library?
- Testeo mas funcional:
    - Este tipo de testing es mas reciliente para refactorizar porque esta mas asociado al comportamiento y no al codigo. Asi que si el codigo cambia en el comportamiento, no es necesario actualizar sus pruebas.
    - Un poco mas dificil de diagnosticar cuando un test falla, en comparacion con un test isolado.

### Aislamiento a la hora de testear

 Esto significa que estas trabajando en un area especifica de tu codigo y por lo tanto si un test falla, sabes rapidamente donde ir.

### Shallow Rendering

- Renderizar componentes solo un nivel de profundidad.
- Renderiza el padre, pero usa placeholder para los hijos.
- Es útil para limitarse a probar un componente como una unidad y para asegurarse de que sus pruebas no afirmen indirectamente el comportamiento de los componentes secundarios.

**Quedemonos con lo siguiente sobre este capitulo: Enzyme** nos proporciona la posibilidad de testear un componente de forma mas isolada/aislada como una unidad. 