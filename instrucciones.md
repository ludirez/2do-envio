desde Ubuntu.
en la carpeta de trabajo, en la consola: 

configuracionde git, nombre de usuario
git config          ->lista de loq ue se peude configurar
git --list
git config --list --show-origin

    1.-verificar nombre de usuario.
        en la terminal: git config --global user.name "nombredeusuariogithub" (incluye comillas)
    2.-verificar correo de usuario.
        en la terminal: git config --global user.email "correoelectronicoregistradoengithub"
    3.-verificar que quedo configurado
        en la terminal: git config --list



rama master
git init                            ->inicia seguimiento de cambios

git status                          ->Muestra que hay para sincronizar con git
                                        mostrara en rojo los pendientes

git add "archivo.extencion"         ->para agregar a cache, el archivo al paquete a sincronizar
                                        mostrara en verde los enlistados een chache

git rm --cached "archivo.extencion"          ->para quetar de la lista mas no borra el archivo del dir

git commit -m "mensaje descriptivo"            ->para subir los enlistados en cache y dejar un
                                                aviso descriptivo de que va o que se hizo