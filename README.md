# Laboratorio-11-Plantilla
1.¿Cuál es la finalidad del archivo vercel.json? 
    R/ Es para que el archivo sea utilizado para configurar y personalizar los despliegues de las aplicaciones en Vercel. Permitiendo especificar las rutas, builds, rewrites y redirects, headers.

2.¿Qué ventajas tiene desplegar en Vercel frente a un servidor tradicional?
    R/ Entre algunas de las ventajas estan la facilidad de uso, estabilidad automática, despliegues rápidos, dominio y HTTPS automáticos

3.¿Qué propiedades del archivo vercel.json son necesarias para que una aplicación Express funcione correctamente en Vercel?
    R/ Para que funcione correctamente debe de llevar la version, los builds, las rutas
    {
  "version": 2,
  "builds": [
    {
      "src": "app.js",
      "use": "@vercel/node"
    }
  ],
  "routes": [
    {
      "src": "/(.*)",
      "dest": "app.js"
    }
  ]
}