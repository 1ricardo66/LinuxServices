### Gerenciar usuarios linux 

```

1. Exibir todos os usuários existentes na rede
    sudo cat /etc/passwd
2. Registrar e deletar usuários
    useradd e adduser
        useradd - Após utilizar o comando é necessário utilizar o "passwd" para delegar uma senha para o user! 
3. Remover usuários
    sudo userdel -r ricardo
       
============================ FLAGS ============================

Options:
  -f, --force                   force some actions that would fail otherwise
                                e.g. removal of user still logged in
                                or files, even if not owned by the user
  -h, --help                    display this help message and exit
  -r, --remove                  remove home directory and mail spool
  -R, --root CHROOT_DIR         directory to chroot into
  -P, --prefix PREFIX_DIR       prefix directory where are located the /etc/* files
  -Z, --selinux-user            remove any SELinux user mapping for the user

==================================================================

4. Criar grupos e adicionar usuários a eles
    addgroup diretores
    addgroup operadores

    Ex: sudo usermod -a -G diretores ricardo

    -a, --append append the user to the supplemental GROUPS
    -G, --groups GROUPS new list of supplementary GROUPS

```
