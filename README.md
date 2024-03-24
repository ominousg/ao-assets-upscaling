# AO assets upscaling

## Stable Diffusion

Agrandamiento y remasterización de varios gráficos del Argentum Online usando un [modelo open-source de Stable Diffusion](https://old.reddit.com/r/StableDiffusion/comments/1bfnia0/magnific_ai_upscaler_has_been_reverse_enginered/) llamado [Clarity Upscaler](https://github.com/philz1337x/clarity-upscaler) que busca emular el modelo closed-source [Magnific AI](https://magnific.ai/). Se puede probar gratis un par de veces en [Replicate](https://replicate.com/philz1337x/clarity-upscaler). Para mejores resultados, primero agrando el gráfico original usando el modelo de ESRGAN 2x_FakeFaith-Lite_105000_G con ChaiNNer y después lo agrando-remasterizo usando Clarity Upscaler. Es decir, el resultado final es 4 veces más grande que el gráfico original, mejorandole la calidad y -algunas veces- remasterizando el diseño con detalles nuevos que el Clarity Upscaler agregó por su cuenta. Clarity también puede hacer downscaling de las imágenes para achicarlas tratando de mantener la calidad y diseño original. Si tu cliente se maneja con pngs sin fondo negro como en el [AOWeb](https://github.com/ominousg/ao-web-client), se puede usar el modelo de [codeplugtech](https://replicate.com/codeplugtech/background_remover) para removerlo.

### Video con comparaciones side-by-side

<a href="https://www.youtube.com/watch?v=T_enS5HZEQE" target="_blank">
 <img src="https://github.com/ominousg/ao-assets-upscaling/blob/main/upscaled_Stable_Diffusion/djinn_comparacion.png?raw=true" alt="Video con comparaciones side-by-side" width="600" />
</a>


### Otros ejemplos

Palmera

![](https://github.com/ominousg/ao-assets-upscaling/blob/main/upscaled_Stable_Diffusion/Palmera.png?raw=true)

Mausoleo

![](https://github.com/ominousg/ao-assets-upscaling/blob/main/upscaled_Stable_Diffusion/Mausoleo.png?raw=true)

Entrada Dungeon Marabel

![](https://github.com/ominousg/ao-assets-upscaling/blob/main/upscaled_Stable_Diffusion/Dungeon_Marabel.png?raw=true)

Piano

![](https://github.com/ominousg/ao-assets-upscaling/blob/main/upscaled_Stable_Diffusion/Piano.png?raw=true)

Arbol 3

![](https://github.com/ominousg/ao-assets-upscaling/blob/main/upscaled_Stable_Diffusion/Arbol_3.png?raw=true)

Escritorio

![](https://github.com/ominousg/ao-assets-upscaling/blob/main/upscaled_Stable_Diffusion/Escritorio.png?raw=true)

Carreta

![](https://github.com/ominousg/ao-assets-upscaling/blob/main/upscaled_Stable_Diffusion/Carreta.png?raw=true)


## ESRGAN (PyTorch)

Probé 60 modelos de upscaling hechos con PyTorch para agrandar los gráficos del AO. Salieron mejor de lo que esperaba pero le falta unos retoques. ~~Capaz en el futuro entrene un modelo para generar resultados mas parecidos al gráfico original~~ ya no es necesario gracias a los modelos fine-tuneados de Stable Diffusion.

Los 4 mejores son: 2x_Gen5-Alpha_175000_G, [2x_Bubble_AnimeScale_SwinIR_Small_v1](https://github.com/Bubblemint864/AI-Models), 2x_FakeFaith-Lite_105000_G y [XbrWasm](https://www.maxlaumeister.com/xbr-wasm/).

### Herramienta: [chaiNNer](https://chainner.app/)

![](https://github.com/ominousg/ao-assets-upscaling/blob/main/upscaled_ESRGAN/ejemplo-chaiNNer.png?raw=true)
Tutorial: [como upscalear todas las imágenes en un directorio](https://youtu.be/FiB8kIgvzok?si=-lXvfUPSm-elB1ef&t=358).

### Ejemplos

Placas +2 - Spritesheet personaje (2x_Gen5-Alpha_175000_G)

![](https://github.com/ominousg/ao-assets-upscaling/blob/main/upscaled_ESRGAN/armadura-spritesheet-upscale.png?raw=true)

Placas +2 - Item

![](https://github.com/ominousg/ao-assets-upscaling/blob/main/upscaled_ESRGAN/armadura-item-upscale.png)

Vestimenta - Spritesheet personaje

![](https://github.com/ominousg/ao-assets-upscaling/blob/main/upscaled_ESRGAN/vestimenta-spritesheet-upscale.png?raw=true)

Vestimenta - Item

![](https://github.com/ominousg/ao-assets-upscaling/blob/main/upscaled_ESRGAN/vestimenta-item-upscale.png?raw=true)

Túnica - Spritesheet personaje

![](https://github.com/ominousg/ao-assets-upscaling/blob/main/upscaled_ESRGAN/tunica-spritesheet-upscale.png?raw=true)

Túnica - Item

![](https://github.com/ominousg/ao-assets-upscaling/blob/main/upscaled_ESRGAN/tunica-item-upscale.png?raw=true)

Liche (2x_Gen5-Alpha_175000_G)

![](https://github.com/ominousg/ao-assets-upscaling/blob/main/upscaled_ESRGAN/liche-upscale.png?raw=true)

Ogro (2x_Gen5-Alpha_175000_G)

![](https://github.com/ominousg/ao-assets-upscaling/blob/main/upscaled_ESRGAN/ogro-upscale.png?raw=true)

Estatua

![](https://github.com/ominousg/ao-assets-upscaling/blob/main/upscaled_ESRGAN/estatua-upscale.png?raw=true)



### Links adicionales:

[/r/GameUpscale](https://old.reddit.com/r/GameUpscale/)

[Upscale Wiki - Model Database](https://upscale.wiki/wiki/Model_Database) - Actualizado: [OpenModelDB](https://openmodeldb.info/)
