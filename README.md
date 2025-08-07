# 📱 MultiTrackingManager - AR Image Tracking com ARFoundation

Este é um script C# desenvolvido para projetos Unity que utilizam o ARFoundation. Ele permite o rastreamento simultâneo de múltiplas imagens de referência usando o componente `ARTrackedImageManager`.

## 🚀 Funcionalidades

- 📸 Rastreia múltiplas imagens ao mesmo tempo.
- 🧱 Instancia objetos (prefabs) associados às imagens detectadas.
- 🎯 Atualiza a posição e rotação dos objetos conforme a imagem rastreada.
- 👻 Oculta objetos quando a imagem não está sendo rastreada.

## 🛠️ Requisitos

- Unity 2020.3 ou superior (recomendado LTS)
- AR Foundation (pacote Unity)
- ARKit (iOS) ou ARCore (Android)
- Câmera com suporte a AR
- Prefabs 3D para exibir sobre as imagens

## 🧩 Como usar

1. Adicione o script `MultiTrackingManager` a um GameObject vazio na cena.
2. Adicione o componente `ARTrackedImageManager` ao mesmo GameObject.
3. Crie uma lista de prefabs (no `Inspector`) e vincule cada prefab a uma imagem de referência correspondente no seu `XR Reference Image Library`.
4. Execute o projeto em um dispositivo com suporte a AR.

## 📂 Estrutura do Script

- `PrefabsToSpawn`: Lista de objetos que serão instanciados.
- `ARTrackedImageManager`: Componente que detecta as imagens.
- `Dictionary<string, GameObject>`: Armazena os objetos instanciados por nome.
- Eventos para adicionar, atualizar e remover imagens rastreadas.

  ---

Desenvolvido com ❤️ usando Unity + ARFoundation.
