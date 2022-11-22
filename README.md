# Work team Git

![image](https://user-images.githubusercontent.com/50744116/203443744-890a2d10-5c1b-494d-836c-4f16f373d926.png)

- Quando começar uma nova funcionalidade (Tarefa)
    - Passo 1: Atualize a sua branch principal (main ou master) com a nova versão do github.
        
        `git pull origin main`
        
    - Passo 2: Crie uma nova branch para sua tarefa - Sugestão de nome do branch
        
        `git checkout -b develop-thi`
        
    - Passo 3: A cada ciclo de trabalho (ou dia), lembre-se comitar e salvar o código no github.
        
        `git add . && git commit -m "um texto descritivo"`
        
        `git push -u origin develop-thi`
        
- Quando terminar a funcionalidade (Tarefa)
    - Passo 1: Salve seu código no github
        
        `git add . && git commit -m "texto descritivo"`
        
        `git push develop-thi`
        
    - Passo 2: Agora vamos mesclar nossa branch na branch principal (main ou master), porém antes vamos garantir que não há conflitos com a versão mais nova da branch principal.
        
        `git checkout main`
        
        `git pull main`
        
    - Passo 3: Vamos até nossa branch e fazemos o merge
        
        `git checkout develop-thi`
        
        `git merge main`
        
    - Passo 4: Verificamos se há conflitos, se existirem devemo corrigi-los e salvar as alterações
        
        `git add . && git commit -m "texto descritivo"`
        
        `git push develop-thi`
        
    - Passo 5: Ufa, agora só precisamos abrir a Pull Request e aguardar.
