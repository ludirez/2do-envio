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

Para despues de cambios en 1 o mas archivos, se deve volver a ahcer el "git add"
pra agregar todos los archisvos cambiados, 
    en consola: git add .    ->donde el "." indica todo dentro del dir

git log "archivo.extencion"  -->mostrara el historial de cambios de el archivo.

mas comandos:
git show "archivo.extencion"  ->sin coillas, mostrara lo que s e ha cambiado

git diff "dumero del comid a" "numeor de comit b"   ->compara a vs b

cada commit es una version de el archivo. con "checkout" se trae devuelta la vercion que encesitesmos con en codigo de numeros largos de cada log. ejemplos proximos

Ramas del proyecto.
    "master" que ahora se llama "main" es la principal
    "development" para probar cosas
    "bugfinxing" llamado ahora "hotfix" para arreglos urgentes
pueden haber muchas mas ramas, lo importante es aprender a hacer "merge" que es la union de las ramas  alternar con al sagrada linea del tiempo principal.

    Volver en el tiempo.
git log                     nos mostrará  todos los comid, selecionamos a donde queremos ir.
                            nos apoyaremos en los mensajes. pore so su importancia.
                            selecionamos el NunCommit al que queremos voler

git reset nunCommit --hard   para volver la la version selecionada y se pierde lo que precedia
                            al NumCommit

git reset nunCommit --soft        