# Criando-uma-Calculadora-de-IMC-Com-Flutter

**Desenvolvendo uma Calculadora de IMC com Flutter: Um Guia Modular**

**Introdução ao Projeto**
O Índice de Massa Corporal (IMC) é uma medida reconhecida mundialmente para avaliar o nível de adequação do peso de uma pessoa em relação à sua altura. Neste projeto, você será guiado através do processo de criação de uma aplicação Flutter que calcula o IMC, oferecendo aos usuários uma ferramenta interativa e educativa.

**Módulo 1: Configuração do Ambiente**
Antes de começarmos a codificar, é essencial preparar o ambiente de desenvolvimento:
- Instale o [Flutter SDK](https://flutter.dev/docs/get-started/install) e o [Dart](https://dart.dev/get-dart).
- Configure seu editor de código preferido com suporte para Flutter e Dart.
- Crie um novo projeto Flutter com o comando `flutter create calculadora_imc`.

**Módulo 2: Estrutura Básica da Aplicação**
A estrutura de uma aplicação Flutter é composta por widgets que definem a interface do usuário:
```dart
import 'package:flutter/material.dart';

void main() => runApp(CalculadoraIMC());

class CalculadoraIMC extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      title: 'Calculadora de IMC',
      theme: ThemeData(
        primarySwatch: Colors.blue,
      ),
      home: TelaPrincipal(),
    );
  }
}
```

**Módulo 3: Design da Interface do Usuário**
A tela principal da calculadora de IMC incluirá campos para entrada de dados e um botão para realizar o cálculo:
```dart
class TelaPrincipal extends StatefulWidget {
  @override
  _TelaPrincipalState createState() => _TelaPrincipalState();
}

class _TelaPrincipalState extends State<TelaPrincipal> {
  // Variáveis e métodos virão aqui
}
```

**Módulo 4: Lógica de Cálculo do IMC**
O cálculo do IMC é realizado dividindo o peso (em quilogramas) pela altura ao quadrado (em metros):
```dart
double calcularIMC(double peso, double altura) {
  return peso / (altura * altura);
}
```

**Módulo 5: Implementação da Lógica de Interface**
Implemente a lógica para capturar as entradas do usuário e exibir o resultado:
```dart
// Adicione TextEditingController e métodos para atualizar a interface aqui
```

**Módulo 6: Testes e Validação**
Teste sua aplicação em diferentes dispositivos e valide as entradas para garantir que os cálculos estejam corretos.

**Conclusão**
Ao final deste desafio, você terá uma aplicação Flutter funcional que calcula o IMC de um usuário, reforçando seus conhecimentos em Dart e práticas de desenvolvimento com Flutter. Lembre-se de revisar e testar cada módulo para garantir a qualidade e a eficácia da sua calculadora de IMC.
