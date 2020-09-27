# Calculo-de-resistencias-para-leds
#include <stdio.h>

int main(){
    float V;
    float I,Rstd,LedB,RoB,VeB;

    printf("Escribe El Voltaje Que Aplicaras En Tu Circuito: ");
    scanf("%f",&V);

    Rstd=(V-1.5)/0.015; //calculo para el led rojo std
    LedB=(V-2.8)/0.02;
    RoB=(V-2)/0.02;
    VeB=(V-3)/0.02;

    printf("La Resistencia Adecuada Para El Led Rojo STD Es %0.1f Ohms\n",Rstd);
    printf("La Resistencia Adecuada Para El Led Blanco Es %0.1f Ohms\n",LedB);
    printf("La Resistencia Adecuada Para El Led Rojo Brillante Es %0.1f Ohms\n",RoB);
    printf("La Resistencia Adecuada Para El Led Verde Brillante Es %0.1f Ohms\n",VeB);

return 0;
}
