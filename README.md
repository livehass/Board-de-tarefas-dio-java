# Board-de-tarefas-dio-java

## Estrutura das Classes

<p align="center">
  <img src="https://github.com/user-attachments/assets/edb0650a-7436-485e-bace-f3bad84fc1f5" alt="image">
</p>


```java

import java.util.List;
import java.util.UUID;

class Board {
    private UUID id;
    private String name;
    private List<BoardColumn> columns;
}

class BoardColumn {
    private UUID id;
    private String name;
    private String kind;
    private int order;
    private List<Card> cards;
}

class Card {
    private UUID id;
    private String title;
    private String description;
}

```
```java

class Board {
  + id: UUID
  + name: String
  + columns: BoardColumn[]
}

class BoardColumn {
  + id: UUID
  + name: String
  + kind: String
  + order: Int
  + cards: Card[]
}

class Card {
  + id: UUID
  + title: String
  + description: String
}
```
