# Alto Crimen: La Paz City

Juego de acción, sneaking y vida callejera ambientado en **La Paz, Bolivia**. Manejá
minibús y taxi, hacé chapu, esquivá a la policía, asaltabos, corréte de Los Cóndores y
subí de rango en tres mapas que cubren toda la ciudad y El Alto.

Todo vive en **un solo archivo HTML**. No hay build, ni dependencias, ni servidor.
Abrilo y a jugar.

## Jugar online

[**Jugar ahora →**](https://hashwar-gif.github.io/alto-crimen-la-paz-city/)

## Jugar en local

Abrí `index.html` en cualquier navegador moderno (Chrome, Edge, Firefox, Safari).

```bash
# O servilo local (recomendado para que el guardado funcione consistente)
python -m http.server 8000
# luego abrí http://localhost:8000
```

En celular también funciona con controles táctiles (joystick + botones en pantalla).
La partida se guarda sola en el navegador con `localStorage`.

## Controles

| Tecla | Acción |
|---|---|
| `↑` `↓` `←` `→` | Mover / conducir |
| `E` | Manejar · volar · comprar C (celular) |
| `ESPACIO` | Frenar / derrapar |
| `F` | Subir de pasajero |
| `J` | Golpe |
| `K` | Disparar |
| `G` | Asaltar |
| `Q` | Cambiar arma |
| `N` | Mapa |
| `R` | Radio |
| `X` | Cancelar misión |
| `P` | Pausa |
| `O` | Opciones |
| `Y` | Jugador 2 |
| `1` `2` `3` | Elegir mapa |

## Música

- **Portada** — al abrir el juego suena el tema *Staley*. En PC arranca solo; en
  el celular el navegador exige un toque, así que aparece el cartel
  *"TOCA LA PANTALLA PARA LA MÚSICA"* hasta que empieza. Se puede apagar desde
  **Opciones → Música en portada**.
- **Radio JDR-IA 100.1 FM** — nueva estación dentro del juego, con los temas
  *Verde adicción*, *Mujer* y *Ojitos lindos*. Solo suena dentro de un vehículo
  y va rotando sola al terminar cada tema. Se prende con la tecla `R` o el botón
  **RADIO** del panel táctil.
- **Opciones** — volumen de música, elegir tema (con anterior / siguiente) y
  apagar la música de portada.

## Modos

- **Nueva historia** — ruta de **9 capítulos** de El Alto a Plaza Murillo. Elegís
  personaje (chofer o bandas) y avanzás según el guion.
- **Juego libre** — toda la ciudad, sin guion, con todas las misiones libres.
- **Continuar** — retoma tu partida guardada.

## Misiones

Ruta de minibús, taxi, entrega de sal y correo, tour al mirador, carreras, encargos
de Don Wilson en el taller, vuelo de avioneta aros incluidos, fiesta y huida de la
policía.

## Mapas

| # | Mapa | Tamaño | Zonas | Estado |
|---|---|---|---|---|
| 1 | Pequeño | 8 × 7 km | La Ceja, Centro, Sopocachi, Miraflores, Obrajes | **Juego completo** |
| 2 | Mediano | 15 × 11,4 km | Suma El Alto (16 de Julio, Río Seco, Villa Adela, aeropuerto), Irpavi, Calacoto, Línea Azul completa | 🔒 Pase Completo |
| 3 | Grande | 18,6 × 13,8 km | Toda La Paz y El Alto: Senkata, aeropuerto internacional, Achumani, Mallasa, Valle de la Luna y la Muela del Diablo | 🔒 Pase Completo |

Esta versión pública trae el **mapa pequeño** completo. Los mapas mediano y grande
aparecen en el selector pero bloqueados; sus datos no forman parte del archivo, así que
la descarga pesa ~1 MB en vez de ~2,9 MB.

## Cómo está hecho

- HTML + CSS + JavaScript puros, canvas 2D, cero dependencias.
- Mapas definidos como base64 dentro del propio archivo, así el juego viaja entero
  en una sola página.
- La web se publica sola con GitHub Actions a GitHub Pages en cada `push` a `main`.

## Licencia

MIT — ver [LICENSE](LICENSE).
