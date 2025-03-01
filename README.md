Dio - Modelando o iPhone com UML: Funções de Músicas, Chamadas e Internet.

#PNG UML Mermaid
![UML_Mermaid](https://github.com/WendelTytan/DIO_UML-Iphone/blob/main/mermaid-diagram-2024-09-24-001823.png?raw=true).

#Codigo UML Mermaid
```mermaid
classDiagram
    class IPhone {

    }

    class ReprodutorMusical {
        -Musica[] musicas
        +tocar(): void
        +pausar(): void
        +selecionarMusica(): void
    }

    class AparelhoTelefonico {
        -Contato[] contatos
        -redeMovelDisponivel(): Boolean
        +ligar(): void
        +atender(): void
        +iniciarCorreioVoz(): void
    }

    class NavegadorInternet {
        -ConexaoComInternet(): Boolean
        +exibirPagina(): void
        +adicionarNovaAba(): void
        +atualizarPagina(): void
    }

    class Musica {
        nome: String
        caminho: String
    }

    class Contato {
        nome: String
        numero: String
    }

    class Walkman {
    }

    class Discman {
    }

    class Nokia3310 {
    }

    class MotorolaRazrV3 {
    }

    class FireFox {
    }

    class Safari {
    }

    IPhone --|> ReprodutorMusical
    IPhone --|> AparelhoTelefonico
    IPhone --|> NavegadorInternet

    ReprodutorMusical --* Musica
    ReprodutorMusical <-- Walkman
    ReprodutorMusical <-- Discman

    AparelhoTelefonico --* Contato
    AparelhoTelefonico <-- Nokia3310
    AparelhoTelefonico <-- MotorolaRazrV3

    NavegadorInternet <-- FireFox
    NavegadorInternet <-- Safari
```
