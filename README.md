# Aula 3 - Refatoração completa

Inclusão do conceito de malha poligonal (mesh). A malha divide-se em duas classes principais:

1. MeshBuilder: Utilizada para construção da malha
1. Mesh: Que representa a malha depois de pronta.

O código representa apenas malhas estáticas, cujos atributos não mudam após sua criação.

Para que os uniforms da malha possam ser guardados em um único map, duas classes auxiliares foram criadas:

1. UniformType: Representando um tipo de uniforme suportado pela malha
1. Uniform: Representando o valor do uniforme e seu tipo.

Observe em especial a criação e desenho (métodos init() e draw()), que agora ficam drasticamente simplificados.