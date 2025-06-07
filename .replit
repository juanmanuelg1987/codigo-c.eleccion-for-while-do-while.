// ============================================================================
//Juan Manuel Garcia
// ============================================================================

#include <stdio.h>
#include <stdlib.h>

#define GREEN   "\x1b[32m"
#define YELLOW  "\x1b[33m"
#define CYAN    "\x1b[36m"
#define RED     "\x1b[31m"
#define RESET   "\x1b[0m"

int main() {
    int opcion;

    do {
        system("clear");
        // Muestra el menú de opciones
        printf("\n" GREEN "========================================\n" RESET);
        printf(GREEN "         MEN\u00da DE EJERCICIOS CON BUCLES\n" RESET);
        printf(GREEN "========================================\n" RESET);
        printf(YELLOW "1.  N\u00fameros del 1 al 10 (for)\n");
        printf("2.  N\u00fameros pares del 2 al 20 (while)\n");
        printf("3.  Suma primeros 10 n\u00fameros (for)\n");
        printf("4.  Pedir n\u00fameros hasta 0 (do-while)\n");
        printf("5.  Calcular factorial (for)\n");
        printf("6.  Contar positivos (while)\n");
        printf("7.  Tabla de multiplicar (for)\n");
        printf("8.  Sumar hasta negativo (do-while)\n");
        printf("9.  N\u00fameros 10 al 1 descendente (for)\n");
        printf("10. Verificar n\u00famero primo (while)\n");
        printf("0.  SALIR\n");
        printf("========================================\n");
        printf(CYAN "Seleccione una opci\u00f3n: " RESET);

        // Lee la opción del usuario
        scanf("%d", &opcion);

        // Switch para ejecutar el ejercicio seleccionado
        switch (opcion) {
            case 1: {
                printf("=== EJERCICIO 1: N\u00fameros del 1 al 10 ===\n");
                for (int i = 1; i <= 10; i++) {
                    printf("%d ", i);
                }
                printf("\n");
                break;
            }

            case 2: {
                printf("=== EJERCICIO 2: N\u00fameros pares del 2 al 20 ===\n");
                int numero = 2;
                while (numero <= 20) {
                    printf("%d ", numero);
                    numero += 2;
                }
                printf("\n");
                break;
            }

            case 3: {
                printf("=== EJERCICIO 3: Suma de primeros 10 n\u00fameros naturales ===\n");
                int suma = 0;
                for (int i = 1; i <= 10; i++) {
                    suma += i;
                    printf("Sumando %d: total = %d\n", i, suma);
                }
                printf("Suma total: %d\n", suma);
                break;
            }

            case 4: {
                printf("=== EJERCICIO 4: Pedir n\u00fameros hasta ingresar 0 ===\n");
                int numero;
                do {
                    printf("Ingrese un n\u00famero (0 para salir): ");
                    scanf("%d", &numero);
                    if (numero != 0) {
                        printf("N\u00famero ingresado: %d\n", numero);
                    }
                } while (numero != 0);
                printf("\u00a1Ejercicio terminado!\n");
                break;
            }

            case 5: {
                printf("=== EJERCICIO 5: Calcular factorial de un n\u00famero ===\n");
                int numero;
                long long factorial = 1;
                printf("Ingrese un n\u00famero para calcular su factorial: ");
                scanf("%d", &numero);

                if (numero < 0) {
                    printf(RED "Error: No se puede calcular factorial de n\u00fameros negativos\n" RESET);
                } else {
                    for (int i = 1; i <= numero; i++) {
                        factorial *= i;
                        printf("%d! parcial = %lld\n", i, factorial);
                    }
                    printf("El factorial de %d es: %lld\n", numero, factorial);
                }
                break;
            }

            case 6: {
                printf("=== EJERCICIO 6: Contar n\u00fameros positivos ===\n");
                int numero;
                int contador = 0;
                printf("Ingrese n\u00fameros (n\u00famero negativo para terminar):\n");

                while (1) {
                    printf("N\u00famero: ");
                    scanf("%d", &numero);

                    if (numero < 0) {
                        break;
                    }

                    if (numero > 0) {
                        contador++;
                        printf("N\u00fameros positivos ingresados hasta ahora: %d\n", contador);
                    }
                }
                printf("Total de n\u00fameros positivos ingresados: %d\n", contador);
                break;
            }

            case 7: {
                printf("=== EJERCICIO 7: Tabla de multiplicar ===\n");
                int numero;
                printf("Ingrese un n\u00famero para ver su tabla de multiplicar: ");
                scanf("%d", &numero);

                printf("\nTabla de multiplicar del %d:\n", numero);
                printf("------------------------\n");
                for (int i = 1; i <= 10; i++) {
                    int resultado = numero * i;
                    printf("%d x %d = %d\n", numero, i, resultado);
                }
                break;
            }

            case 8: {
                printf("=== EJERCICIO 8: Sumar n\u00fameros hasta ingresar negativo ===\n");
                int numero;
                int suma = 0;
                printf("Ingrese n\u00fameros para sumar (n\u00famero negativo para terminar):\n");

                do {
                    printf("N\u00famero: ");
                    scanf("%d", &numero);

                    if (numero >= 0) {
                        suma += numero;
                        printf("Suma parcial: %d\n", suma);
                    }
                } while (numero >= 0);

                printf("Suma total: %d\n", suma);
                break;
            }

            case 9: {
                printf("=== EJERCICIO 9: N\u00fameros del 10 al 1 (descendente) ===\n");
                for (int i = 10; i >= 1; i--) {
                    printf("%d ", i);
                }
                printf("\n");
                break;
            }

            case 10: {
                printf("=== EJERCICIO 10: Verificar si un n\u00famero es primo ===\n");
                int numero;
                int esPrimo = 1;

                printf("Ingrese un n\u00famero para verificar si es primo: ");
                scanf("%d", &numero);

                if (numero <= 1) {
                    esPrimo = 0;
                } else if (numero == 2) {
                    esPrimo = 1;
                } else {
                    int divisor = 2;
                    while (divisor * divisor <= numero && esPrimo) {
                        if (numero % divisor == 0) {
                            esPrimo = 0;
                            printf("Divisor encontrado: %d\n", divisor);
                        }
                        divisor++;
                    }
                }

                if (esPrimo) {
                    printf("El n\u00famero %d ES PRIMO\n", numero);
                } else {
                    printf("El n\u00famero %d NO ES PRIMO\n", numero);
                }
                break;
            }

            case 0:
                printf("\u00a1Gracias por usar el programa!\n");
                break;

            default:
                printf(RED "Opci\u00f3n inv\u00e1lida. Intente nuevamente.\n" RESET);
        }

        // Pausa para que el usuario pueda ver los resultados
        if (opcion != 0) {
            printf("\nPresione Enter para continuar...");
            getchar(); // Consume el \n del scanf anterior
            getchar(); // Espera que el usuario presione Enter
        }

    } while (opcion != 0);

    return 0;
}

// ============================================================================
//Juan Manuel Garcia
