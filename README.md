# atm_consultoria

A new Flutter project.

## Getting Started

This project is a starting point for a Flutter application.

A few resources to get you started if this is your first Flutter project:

- [Lab: Write your first Flutter app](https://flutter.dev/docs/get-started/codelab)
- [Cookbook: Useful Flutter samples](https://flutter.dev/docs/cookbook)

For help getting started with Flutter, view our
[online documentation](https://flutter.dev/docs), which offers tutorials,
samples, guidance on mobile development, and a full API reference.

# ATM Consultoria Recursos Utilizados

## Image Assets

Após criar uma pasta com as imagens desejadas é necessário adicionar  o caminho delas no <em>pubspec.yaml</em>  e definir uma sessão chamada assets logo em seguida adicione o caminho das imagens separados como no exemplo:
```
assets: 
  - imagens/cliente1.png 
  - imagens/cliente2.png
```

Para utilizar dentro de uma classe é necessário usar o Widget Image.asset("caminho/imagem.png")
```
Image.asset("imagens/logo.png")
```

## GestureDetector

O "Gesture detector" é um Widget responsável pela identificação de toques em outro determinado Widget, em o que vai ser determinado o gesto é definido no child do Widget e o tipo de gesto a ser detectado também, junto com esse atributo é definido o método que será executado no momento que for realizado o clique. 
```
GestureDetector( 
   onTap: _abrirEmpresa, 
   child: Image.asset("imagens/menu_empresa.png"), 
),
```

Troca de Tela
Como alterar entre diferentes telas em aplicativos em Flutter, pode ser usado o "Navigator.push"

```
Navigator.push(
context,
MaterialPageRoute(builder: (context)=> Tela() ));
```
