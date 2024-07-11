# ssh-keys
Como gerar chaves ssh e adicionar ao servidor

# Exportar chaves no linux
  1 - No terminal cliente executar:
      ssh-keygen -b 4096 (para gerar as chaves privadas e publicas no caminho ~/.ssh/)
        
        Séra solicitado informar o local onde o arquivo será gravado.
        ![image](https://github.com/FOvidio/ssh-keys/assets/148785762/dc0f1e0a-0bd7-4c5d-809e-3d7cf18d81a2)
        
        Em seguida é solicitada uma frase de segurança (Não informar), apenas tecle Enter 2 vezes.
        ![image](https://github.com/FOvidio/ssh-keys/assets/148785762/9ea3a395-6969-4ccc-a034-2094af24834a)


       Comando para listar os arquivos, (ls -l ~/.ssh/)
       ![image](https://github.com/FOvidio/ssh-keys/assets/148785762/d31935dd-3d9b-48dc-b219-8c74b7987b09)


  2 - Transferir a chave publica para o servidor
      ssh-copy-id usuário@192.168.1.XX >> 
      Este comando envia o arquivo ao servidor e adiciona a chave ao ~/.ssh/
