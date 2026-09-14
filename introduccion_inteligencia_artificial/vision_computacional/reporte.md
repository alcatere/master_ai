 - ¿Qué clases detectó YOLO en las fotos de Ultralytics y cuáles en la tuya?
En mi caso detecto a las 3 personas que habia en la foto, detecto una flor, el contenedor de la flor e indico un una manzana que en realidad es un globo, este siendo le unico error de detección, teniendo en cuenta que lo clasifico con un 23% de confianza.

- ¿Algún objeto evidente de tu foto no salió etiquetado? ¿Por qué podría pasar (clase que no está en COCO, objeto chico, recorte, umbral de confianza)?
En CLI no obtuvo la otra flor con su contenedor ni el pastel

- ¿La predicción de la celda CLI y la de model(...) coinciden sobre tu misma imagen?
No son la misma, ya que model(...) detecto a las 3 personas, 2 flores, 2 contenedores de la flor, mientras que en CLI solo detecto a las 3 personas y un contenedor de la flor, con la flor