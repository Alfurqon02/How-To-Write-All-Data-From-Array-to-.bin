# How-To-Write-All-Data-From-Array-to-.bin
12/11/2021


looping sesuai dengan data array yang diisi

      #include <stdio.h>

      int tes[100] = {1, 2, 3, 4, 5};

      int main(){
          FILE *f;
          int i;
          f = fopen ("coba.bin", "wb");
          for(i=0;i<5; i++){
              fwrite(tes, sizeof(int), 1, f);
          }
          fclose(f);
          return 0;
      }

