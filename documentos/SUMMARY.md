
## Sumário

### [Layouts](https://developer.android.com/guide/topics/ui/declaring-layout)

| Tipos de Layouts | Descrição |
| ------------- |-------------|
| ScrollView| Uma View Group que possibilita fazer o scroll da view filha. |
| FrameLayout | O FrameLayout é capaz de exibir uma view por vez, caso tenha mais de uma view elas são sobrepostas.  |
| [LinearLayout](https://developer.android.com/guide/topics/ui/layout/linear) | Layout que organiza os filhos em uma única linha horizontal ou vertical. |
| [~~RelativeLayout~~](https://developer.android.com/guide/topics/ui/layout/relative) | Permite especificar a localização de objetos filhos relativos entre si (filho A à esquerda do filho B) ou relativos aos pais |
| [ConstraintLayout](https://developer.android.com/training/constraint-layout) | "Similar ao `RelativeLayout`... mas é mais flexível e mais fácil de usar com o Android Studio Layout Editor." |
| [~~ListView~~](https://developer.android.com/reference/android/widget/ListView) | Exibe uma coleção de Views roláveis verticalmente, onde cada view é posicionada imediatamente abaixo da view anterior na lista.|  
| [RecyclerView](https://developer.android.com/guide/topics/ui/layout/recyclerview) | Exibe uma coleção de Views em lista ou grid. É mais flexível, customizável e performática do que a ListView. |

#### ConstraintLayout

**Vantagens**

- Otimizado para hierarquias de exibição.
- Você não terá problemas se o estado de visibilidade da sua view for GONE, o alinhamento funcionará mesmo assim e você não vai mais se preocupar com layouts quebrados.
- Editor completamente amigável.
- Fácil de usar e feito para desenhar telas responsivas.

**Desvantagens**

- O layout editor vai simplesmente mover suas views sem motivo algum, isso deve ser causado quando tentamos mover uma view e acabamos clicando em outra.
- Performance. A performance em que as views são criadas é um pouco inferior se comparar ao RelativeLayout ou LinearLayout. Veja este caso: [ConstraintLayout Performance](https://medium.com/@krpiotrek/constraintlayout-performance-c1455c7984d7).

### [Resources](https://developer.android.com/guide/topics/resources/available-resources)

| Tipos de Resources        | Descrição           |
| ------------- |-------------|
| Layout | Defina o layout para a interface do usuário da aplicação. `res/layout/` |
| String | Define strings, arrays, e plurais. `res/values/strings` `res/values/arrays` |
| Color | Recurso com valor de cor em hexadecimal `res/colors` |
| Dimension | Recurso com valor de dimensões. Unidade de medidas (dp, sp, ..) `res/dimens`|
| Style | Definição de estilos e formatos para os componentes visuais. `res/style`|
| Menu | Define o conteúdo dos menus do seu aplicativo `res/menu`|
| Drawable | Recurso de "desenhos" como bitmaps, XML de gráficos `res/drawable/` |

### Tips and Tricks
- Padrão de nomeclatura dos arquivos de layouts;
- Padrão de IDs dos componentes no XML;
- Re utilizando Layouts com [include](https://developer.android.com/training/improving-layouts/reusing-layouts);
- Atributo: [tools](https://developer.android.com/studio/write/tool-attributes);
