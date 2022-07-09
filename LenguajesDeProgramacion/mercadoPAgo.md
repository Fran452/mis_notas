# Mercado Pago
## ¿Que es?
Es la pasarela de pago con mayor utilidad en latino america
## Formas de utilizarse
1. Checkout API
Usa las APIs para construir tu propia experiencia de pago en tu sitio web o aplicación móvil. Desde configuraciones básicas a avanzadas, tú controlas la experiencia.
2. Link de pago
Es una solución de cobro práctica y rápida que te permite vender online sin necesidad de tener conocimientos técnicos o de programación
3. Checkout Pro (Utilizada en esta documentacion)
Es una solución que permite a tus clientes realizar compras a través del formulario web de Mercado Pago. 

## Aplicacion general
1. Crearte una cuenta de mercado pago (cliente)
2. Instalar SDK de MP: npm start mercadopago (programador)
3. Tener la credenciales (Cliente)

## Estrucutura
1. Descargar sdk con `npm i mercadopago`
2. Lo requerimos:  `const mercadoPago = require("mercadopago")`
3. Guardamos las credenciales: `const credential = proess.env.MP || "credencial"`
4. Guardamos el server: `let server = process.env.SERVER || linkDelServer`
5. Guardamos el feedback: 
```js
const feedback = `${server}/checkout/feedback`
``` 
6. creamos la estructura de mp:
```js
const mp = async (items,cuotes,) => {
    try{
        mercadoPAgo.configure({
            access_token: credential
        })
        let config = {
            items: item,
            back_urls:{
                success: feedback
                failure: feedback
                pendgin: feedback
            },
            payment_methods : {
                installmentes : cuotes
            },
            auto_return: "approved",
        };

        let preference = await mercadoPAgo.preference.create(config);
        return preference;

    } catch (error){
        throw new Error(error);
    }
}
```

Mas propiedades para la configurancion ingresando aqui: [Mercado Libre](#https://www.mercadopago.com.ar/developers/es/reference/preferences/_checkout_preferences/post)

## Utilizacion
para utilizarlo primero lo requerimos en el controller necesario y luego se le agrega el nombre con el que se requirio y entre parentesis los campos aneriormente seleccionado. Y el link se guarda en el producto y en la propiedad `.init_point`. y se almacena informacion en req.query la operacion para mostrar al usuario.

## Objeto Producto
El objeto que utilizara MP para el pago utiliza la siguiente estructura:
```js
let producto = {
      "title": "Dummy Title",
      "description": "Dummy description",
      "picture_url": "http://www.myapp.com/myimage.jpg",
      "category_id": "car_electronics",
      "quantity": 1,
      "currency_id": "U$",
      "unit_price": 10
    }
```
|propiedad|utilizacion|
|:--:|----------------|
|title| nombre del producto
|description| descripcion del producto
|picture_url| foto del producto en base al link
|category_id| categoria del producto
|quantity| cantidad del producto (__obligatorio__)
|currency_id| moneda en la cual se cobra el producto (__obligatorio__)
|unit_price| precio del producto (__obligatorio__)