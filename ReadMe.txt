

bash: mkfs.msdos: command not found

          sudo apt-get update && apt-get updgrade

          apt-get install dosfstools

          echo $PATH

If it's empty, You may set the PATH variable with this command

          export PATH="$PATH:/usr/local/sbin:/usr/local/bin:/sbin:/bin:/usr/sbin:/usr/bin:/root/bin"


Use thiese command for run the JOSH-OS
          nasm -elf64 kernel.asm -o kernel.bin -f bin
          nasm -elf64 boot.asm -o boot.bin -f bin

          cd /media
          sudo mkdir myfloppy

          mkfs.msdos -C myfloppy.img 1440 

          sudo mount -o loop myfloppy.img /media/myfloppy/

          df -h


          sudo dd if=./boot.bin of=/dev/loop8

          sudo cp kernel.bin /media/myfloppy/

          ls -l /media/myfloppy/
          sudo umount /media/myfloppy/
          sudo rm -rf /media/myfloppy/