## Checkpoint

### INFORMAÇÕES DO ALUNO (Individual)

Nome: ________________________________  
RM: _________________________________  

Modifique o arquivo `main.py` para processar um frame do vídeo, identificar a nave principal e os tiros. O código deve **contar o número total de tiros que atingiram a nave** ao longo do vídeo.


## Regras gerais

- **CP individual.**
- A prova contém **1 questão**.

## Configuração do ambiente

1. **Criar a virtualenv**:

   ```bash
   python3 -m venv venv
   ```

2. **Ativar o ambiente**:

   - macOS / Linux:

     ```bash
     source venv/bin/activate
     ```
   - Windows:

     ```bash
     venv\Scripts\activate.bat
     ```

3. **Instalar as dependências**:

   ```bash
   pip install -r requirements.txt
   ```

## Testar a infraestrutura

- Execute o script de exemplo:

  ```bash
  python main.py
  ```
  Uma janela mostrará a transmissão da câmera. Pressione `q` para sair. Como pode observar, o arquivo `main.py` já carrega um video, mas não estão fazendo nada.

## Importante

No vídeo existem:

- Uma nave principal que deve ser monitorada.
- Tiros que podem ou não atingir a nave.

O desafio é contar o número total de tiros que atingiram a nave principal ao longo do vídeo.

## Saída esperada

Em cada frame processado, escreva na imagem o número de colisões detectadas até aquele momento. Ao final do vídeo, imprima no terminal o número total de colisões detectadas.

## Restrições

- A nave alvo, pode variar de formato em vídeos diferentes.
- Os tiros podem ou não colidir com a nave.
- `O programa deve funcionar mesmo se a nave principal estiver em posições diferentes no vídeo`.
- Considere que um tiro atingiu a nave se houver uma sobreposição significativa entre o tiro e a nave em um frame.

## Rúbrica

1. Nota: 2 - O método consegue identificar a nave e os tiros (desenhe os contornos para validar).
2. Nota: 3 - O programa consegue identificar colisões e contar a quantidade de tiros que atingiram a nave, mas o valor final está incorreto. Ele também mostra o número de colisões na imagem.
3. Nota: 5 - O método contabiliza precisamente o número total de tiros que acertaram a nave principal, para qualquer vídeo com as mesmas características, e exibe o número de colisões na imagem.
