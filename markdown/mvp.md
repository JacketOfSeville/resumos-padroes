# MVP
O padrão MVP (Model-View-Presenter) é uma variação do MVC, amplamente utilizado em desenvolvimento de interfaces de usuário em plataformas como Android e desktop. Ele separa a lógica de negócios da interface de forma distinta:

- **Model (Modelo):** Gerencia dados e lógica de negócios, manipulando interações com bancos de dados ou APIs.
- **View (Visão):** Exibe a interface e captura interações do usuário, mas não interage diretamente com o Model.
- **Presenter (Apresentador):** Intermediário entre View e Model. Recebe entradas da View, processa essas entradas, interage com o Model e atualiza a View com os dados resultantes.

**Fluxo de Trabalho no MVP:**
1. O usuário interage com a View.
2. A View repassa as interações para o Presenter.
3. O Presenter processa as interações, manipula os dados no Model e atualiza a View.

**Vantagens do MVP:**
- **Separação de responsabilidades:** Facilita manutenção e evolução do código.
- **Testabilidade:** O Presenter pode ser testado isoladamente, sem depender da interface gráfica.
- **Flexibilidade:** A View é mais simples e reutilizável, com menos lógica de negócios.

**Comparação com MVC:**
- No MVC, o Controller não conhece a View diretamente; no MVP, o Presenter interage diretamente com a View, oferecendo maior flexibilidade.
- A View no MVP é mais focada na apresentação, enquanto no MVC, pode ter mais responsabilidades.

O padrão MVP é ideal para aplicações que necessitam de alta testabilidade e uma clara separação entre lógica de negócios e interface, como em aplicativos móveis e de desktop.