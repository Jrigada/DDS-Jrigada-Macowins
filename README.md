# DDS-Jrigada-Macowins

## Requerimientos
1. Conocer el precio de venta
2. Conocer el tipo de prenda
3. Conocer las ventas de X dia


```
CLASE PRENDA
  Privado:
    VAR tipo
    VAR estado: T_ESTADO

  Publico: 
    FUNCION precio()
    //retorna el precio de una prenda dependiendo de su estado interno comunicandose con la clase T_ESTADO
    FIN FUNCION
    
FIN CLASE
    
CLASE T_ESTADO
    Privado: 
        VAR precioBase
        VAR descuento
        
    Publico: 
      FUNCION nuevo()
        return precioBase
      FIN FUNCION
      
      
      FUNCION promocion()
        return precioBase - descuento
      FIN FUNCION
      
      
      FUNCION liquidacion()
        return (precioBase/2)
      FIN FUNCION
    
FIN CLASE

CLASE VENTA
  Privado: 
    VAR cantidad
    VAR prendas []
    VAR fecha
    VAR tipo: T_VENTA
    
  Publico: 
    FUNCION ventasDelDia()
    FIN FUNCION
    
    FUNCION vender()
    //calculo de precio trabajando sobre el array de prendas para conocer su precio y aplicando el recargo o no de acuerdo al tipo de venta
    
FIN CLASE

CLASE T_VENTA
    Publico: 
    FUNCION tarjeta()
      //agregar recargo por tarjeta
    FIN FUNCION
    
    FUNCION efectivo()
    FIN FUNCION
    
FIN CLASE



```

![photo_2021-04-15_21-58-58](https://user-images.githubusercontent.com/62958725/114956760-e8231280-9e35-11eb-981e-d3b24f44016e.jpg)
