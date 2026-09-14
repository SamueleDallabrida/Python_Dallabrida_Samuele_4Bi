## Configurazione Git

- Comandi usati:

1. git config --global user.name "Samuele Dallabrida"
2. git config --global user.mail "samuele.dallabrida09@marconirovereto.it"
3. git config --global init.defaultBranch main
4. git config --global core.editor "code"
5. git config --list --show-origin <!--comando per visualizzare tutte le azioni precedenti-->

- Output:
  - file:/etc/gitconfig     user.email=samuele.dallabrida09@marconirovereto.it  
    file:/etc/gitconfig     gpg.program=/.codespaces/bin/gh-gpgsign  
    file:/etc/gitconfig     init.defaultbranch=main  
    file:/etc/gitconfig     credential.helper=/.codespaces/bin/gitcredential_github.sh  
    file:/home/codespace/.gitconfig filter.lfs.clean=git-lfs clean -- %f  
    file:/home/codespace/.gitconfig filter.lfs.smudge=git-lfs smudge -- %f  
    file:/home/codespace/.gitconfig filter.lfs.process=git-lfs filter-process  
    file:/home/codespace/.gitconfig filter.lfs.required=true  
    ```file:/home/codespace/.gitconfig user.name=Samuele Dallabrida  
    file:/home/codespace/.gitconfig user.email=samuele.dallabrida09@marconirovereto.it  
    file:/home/codespace/.gitconfig init.defaultbranch=main  
    file:/home/codespace/.gitconfig core.editor=code```  
