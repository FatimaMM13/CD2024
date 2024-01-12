- Las razones para seleccionar un IDE concreto:

He escogido NetBeans porque he utilizado este programa y es sencillo de utilizar para programar

- El proceso de instalación:

1.Actualiza la lista de apt y instalar los requisitos para instalar NetBeans: Instalar en la terminal
    -> sudo apt update
    -> sudo apt install default-jdk
2.Descargar el archivo Netbeans: En la terminal
    -> sudo wget https://downloads.apache.org/netbeans/netbeans/20/netbeans-20-bin.zip
3.Extraiga el archivo zip de Netbeans: En la terminal
    -> unzip netbeans-20-bin.zip
4.Ajuste la RUTA de los archivos de NetBeans: En la terminal
    -> sudo mv netbeans/ /opt/
5.Abra el archivo ‘~/.bashrc’ en cualquier herramienta de edición de código fuente: En la terminal
    -> sudo nano ~/.bashrc
6.Pegue la ruta dada al final del archivo de la siguiente manera: En la terminal
    -> export PATH="$PATH:/opt/netbeans/bin/"
7.Ahora, obtenga el archivo a través del siguiente comando: En la terminal
    -> source ~/.bashrc
8.Cree un iniciador de escritorio para Netbeans IDE: En la terminal
    -> sudo nano /usr/share/applications/netbeans.desktop
9.Pegue las siguientes líneas dentro del archivo: Anuncio
    -> [Desktop Entry]
        Name=Netbeans IDE
        Comment=Netbeans IDE
        Type=Application
        Encoding=UTF-8
        Exec=/opt/netbeans/bin/netbeans
        Icon=/opt/netbeans/nb/netbeans.png
        Categories=GNOME;Application;Development;
        Terminal=false
        StartupNotify=true
10.Inicie NetBeans IDE en Ubuntu: En la terminal
    -> netbeans

-La compilación o interpretación de un programita sencillo
Programa:
    class HelloWorld {
        public static void main (String args[]) {
            System.out.println("Hello World");
        }
    }