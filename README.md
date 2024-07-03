#include <stdio.h>

int main() {
    int pilihan;
    char lanjut;
    double total = 0.0;
    int count = 0; 
    const int MAX_PESANAN = 10; 
    int pesanan[MAX_PESANAN]; 
    double harga[MAX_PESANAN]; 
    char namaPembeli[100]; 

    printf("Annyeonghaseyo Yeoreobun...\n");
    printf("Selamat datang di Celestial Kpop, destinasi utama Anda untuk koleksi lightstick eksklusif dari berbagai boygroup, girlgroup, dan solois favorit Anda dalam industri Kpop. Di sini, kami menyediakan berbagai pilihan lightstick resmi yang dipersembahkan dengan cinta dan dedikasi untuk memenuhi kebutuhan penggemar sejati musik Kpop.\n");
    getchar();
    
    printf("Masukkan nama Anda: ");
    fgets(namaPembeli, sizeof(namaPembeli), stdin);

    do {
        printf("================================\n");
        printf("Pilihan Lightstick:\n");
        printf("================================\n");
        printf("1. Seventeen   harga Rp. 750.000\n");
        printf("2. BTS         harga Rp. 770.000\n");
        printf("3. EXO         harga Rp. 800.000\n");
        printf("4. GOT7        harga Rp. 700.000\n");
        printf("5. Twice       harga Rp. 650.000\n");
        printf("6. Newjeans    harga Rp. 680.000\n");
        printf("7. Blacpink    harga Rp. 850.000\n");
        printf("8. G-idle      harga Rp. 720.000\n");
        printf("9. IU          harga Rp. 870.000\n");
        printf("10. Zico       harga Rp. 600.000\n");
        printf("================================\n");
        
        printf("Masukan pilihan anda: ");
        scanf("%d", &pilihan);

        switch (pilihan) {
            case 1:
                printf("Anda Memilih Lightstick Seventeen\n");
                printf("Harga Rp. 750.000\n");
                pesanan[count] = 1; 
                harga[count] = 750000; 
                total += 750000;
                count++;
                break;
            case 2:
                printf("Anda Memilih Lightstick BTS\n");
                printf("Harga Rp. 770.000\n");
                pesanan[count] = 2;
                harga[count] = 770000;
                total += 770000;
                count++;
                break;
            case 3:
                printf("Anda Memilih Lightstick EXO\n");
                printf("Harga Rp. 800.000\n");
                pesanan[count] = 3;
                harga[count] = 800000;
                total += 800000;
                count++;
                break;
            case 4:
                printf("Anda Memilih Lightstick GOT7\n");
                printf("Harga Rp. 700.000\n");
                pesanan[count] = 4;
                harga[count] = 700000;
                total += 700000;
                count++;
                break;
            case 5:
                printf("Anda Memilih Lightstick Twice\n");
                printf("Harga Rp. 650.000\n");
                pesanan[count] = 5;
                harga[count] = 650000;
                total += 650000;
                count++;
                break;
            case 6:
                printf("Anda Memilih Lightstick Newjeans\n");
                printf("Harga Rp. 680.000\n");
                pesanan[count] = 6;
                harga[count] = 680000;
                total += 680000;
                count++;
                break;
            case 7:
                printf("Anda Memilih Lightstick Blackpink\n");
                printf("Harga Rp. 850.000\n");
                pesanan[count] = 7;
                harga[count] = 850000;
                total += 850000;
                count++;
                break;
            case 8:
                printf("Anda Memilih G-idle\n");
                printf("Harga Rp. 720.000\n");
                pesanan[count] = 8;
                harga[count] = 720000;
                total += 720000;
                count++;
                break;
            case 9:
                printf("Anda Memilih Lightstick IU\n");
                printf("Harga Rp. 870.000\n");
                pesanan[count] = 9;
                harga[count] = 870000;
                total += 870000;
                count++;
                break;
            case 10:
                printf("Anda Memilih Lightstick Zico\n");
                printf("Harga Rp. 600.000\n");
                pesanan[count] = 10;
                harga[count] = 600000;
                total += 600000;
                count++;
                break;
            default:
                printf("Pilihan tidak valid\n");
        }

        printf("===================================================\n");
        printf("Apakah Anda ingin memesan lightstick lagi? (y/n): ");
        scanf(" %c", &lanjut);
        getchar(); 
        
    } while (lanjut == 'y' || lanjut == 'Y');

    printf("\n\n=============== Struk Pembelian ===============\n");
    printf("================================================\n");
    printf("Atas Nama: %s", namaPembeli); 
    printf("================================================\n");
    printf("No  Nama Lightstick             Harga\n");
    printf("================================================\n");
    
    for (int i = 0; i < count; ++i) {
        switch (pesanan[i]) {
            case 1:
                printf("%d. Lightstick Seventeen       Rp. 750.000\n", i + 1);
                break;
            case 2:
                printf("%d. Lightstick BTS             Rp. 770.000\n", i + 1);
                break;
            case 3:
                printf("%d. Lightstick EXO             Rp. 800.000\n", i + 1);
                break;
            case 4:
                printf("%d. Lightstick GOT7            Rp. 700.000\n", i + 1);
                break;
            case 5:
                printf("%d. Lightstick Twice           Rp. 650.000\n", i + 1);
                break;
            case 6:
                printf("%d. Lightstick Newjeans        Rp. 680.000\n", i + 1);
                break;
            case 7:
                printf("%d. Lightstick Blackpink       Rp. 850.000\n", i + 1);
                break;
            case 8:
                printf("%d. Lightstick G-idle          Rp. 720.000\n", i + 1);
                break;
            case 9:
                printf("%d. Lightstick IU              Rp. 870.000\n", i + 1);
                break;
            case 10:
                printf("%d. Lightstick Zico            Rp. 600.000\n", i + 1);
                break;
            default:
                break;
        }
    }
    printf("================================================\n");
    printf("Total Harga                   Rp %.2f\n", total);
    printf("================================================\n");

    return 0;
}
