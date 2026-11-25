# Gráficos propios del Atlas

Gráficos calculados para el Atlas con datos verificables. Se regeneran con `python3 scripts/graficos/sp1.py`, `python3 scripts/graficos/ppn.py` `python3 scripts/graficos/termo1.py` (este necesita CoolProp) `python3 scripts/graficos/maqel1.py`, `python3 scripts/graficos/mat1.py` `python3 scripts/graficos/electro1.py` (este necesita schemdraw) `python3 scripts/graficos/inst1.py` (también con schemdraw) `python3 scripts/graficos/mec1.py` `python3 scripts/graficos/hidneu1.py` (necesita scipy) y `python3 scripts/graficos/hid2.py` `python3 scripts/graficos/sp2.py` `python3 scripts/graficos/arqnav1.py` (necesita shapely) `python3 scripts/graficos/tecmec1.py` `python3 scripts/graficos/met2.py` `python3 scripts/graficos/lci.py` (CoolProp); los cálculos están registrados en `docs/VERIFICACION.md`.

Convención de colores de Sistemas de Propulsión (pedido del autor, 16/11/2026): empuje en rojo, velocidad del buque en verde, Npe en azul, Neje en amarillo y rendimiento de propulsión en celeste a trazos.

| Archivo | Artículo / sección | Datos | Reemplaza a |
|---|---|---|---|
| sp1-c5-potencia-casco.png | sp1-c5-helice / potencia-casco | Remolcador de la clase (Cátedra de SP); ley del cubo; Cx extra ilustrativos | sp1-c5-potencia-casco.jpg y sp1-c5-np-npe.jpg |
| sp1-c5-curvas-resbalamiento.png | sp1-c5-helice / influencia-s | Serie B de Wageningen B4-70, P/D = 1 (Oosterveld y van Oossanen, 1975); n y H del remolcador | sp1-c5-curvas-resbalamiento.jpg |
| sp1-c5-paso-casco.png | sp1-c5-helice / influencia-s | Serie B de Wageningen B4-70, P/D 0,9 · 1,0 · 1,1; motor de cupla constante (simplificación) | sp1-c5-paso-casco.jpg |
| sp1-c5-mu-alfa.png | sp1-c5-helice / remolque | Esquemático según la cátedra | sp1-c5-mu-alfa.jpg |
| g04-ciclos-reales-angulo.png | g04-ciclos-reales / angulo | Modelo de ciclo del Atlas (src/core/diesel.ts), ilustrativo | g04-ciclos-reales-angulo-1.jpg |
| g15-levas-real.png | g15-levas / real | Ley polinómica 3-4-5, ilustrativa | g15-levas-real-1.jpg |
| camaras-combustion-diesel-inyectores.png | camaras-combustion-diesel / inyectores | Esquema sin escala (lámina de Bosch) | camaras-combustion-diesel-inyectores-2.jpg |
| ppn-toma-carga.png | diesel-conduccion / cat-toma-carga | Puntos de la lámina de Vernière (PPN 2026) | ppn-curva-toma-carga.jpg |
| ppn-campo-potencia.png | diesel-carga / m140-reduccion | Esquemático según el manual PC 2-5V; ley del cubo en ejes logarítmicos | diesel-carga-pc2-campo.jpg |
| ppn-escape.png | diesel-fallas / escape | 16 lecturas de la lámina de Vernière (PPN 2026), ± 2 °C | diesel-fallas-escape-1.jpg |
| ppn-avance-excesivo.png | diesel-fallas / ing-balanceo | Modelo de ciclo del Atlas, avance 25° frente a 15°, ilustrativo | ppn-bal-avance-excesivo.jpg |
| ppn-poco-avance.png | diesel-fallas / ing-balanceo | Modelo de ciclo del Atlas, avance 5° frente a 15°, ilustrativo | ppn-bal-poco-avance.jpg |
| ppn-orden-encendido-16v.png | diesel-conduccion / cat-inversion | Órdenes de encendido EB y BB de la lámina de Vernière (PPN 2026) | (nuevo; la lámina del distribuidor queda) |
| tg-cambio-olympus-tyne.png | tg-conduccion / performance | Lámina de Oga (SP Máquinas 2026), valores aproximados | tg-conduccion-performance-1.jpg |

Convención de colores de Termodinámica (la de las láminas de la cátedra, v0.94.0): adiabática o isentrópica en rojo, presión constante en naranja, volumen constante en violeta, temperatura constante en celeste y trabajo en verde.

| Archivo | Artículo / sección | Datos | Reemplaza a |
|---|---|---|---|
| te-g-politropicas.png | te-c2-procesos / politropicos (y portada) | Aire, gas ideal, desde 1 bar y 300 K; ejemplo n = 1,2 de 1 a 8 bar | te-politropicos.jpg |
| te-g-carnot-vapor.png | te-c3-carnot (y portada) | Agua IAPWS-IF97 (CoolProp), 10 bar y 0,1 bar tomados para el ejemplo | te-carnot-vapor.jpg |
| te-g-maquinas-carnot.png | te-c3-carnot | Esquema de bloques | te-maquina-frigorifica.jpg |
| te-g-carnot-gas-ts.png | te-c4-entropia (y portada) | Aire 600/300 K; V2 = 2·V1 tomado para el ejemplo | te-carnot-ts.jpg (rotulada «T-s» con ejes log p–h) |
| te-g-turbina-hs.png | te-c4-entropia | Agua IAPWS-IF97; 40 bar, 400 °C → 0,1 bar, ηs = 0,85 tomados para el ejemplo | te-turbina-hs.jpg |
| te-g-otto.png | te-c5-ciclos-gas | r = 8; 1 bar, 300 K; q = 1000 kJ/kg tomado para el ejemplo | te-otto-pv.jpg |
| te-g-diesel.png | te-c5-ciclos-gas | r = 18, rc = 2; 1 bar, 300 K | te-diesel-pv.jpg |
| te-g-dual.png | te-c5-ciclos-gas | r = 16, rpv = 1,5, rc = 1,6; Otto y Diesel con igual r y calor | te-dual-pv.jpg |
| te-g-brayton.png | te-c5-ciclos-gas | rp = 5, 10, 20; 300 K y 1400 K (tomado para el ejemplo) | te-brayton-pv.jpg |
| te-g-planta-frigorifica.png | te-c6-frigorifico (y portada) | Esquemático | te-compresion-vapor.jpg |
| te-g-r134a-ph.png | te-c6-frigorifico | R-134a (CoolProp, referencia ASHRAE); 0 °C y 26 °C, ejemplo de Moran-Shapiro | te-compresion-ph.jpg |
| me-g-trafo-circuito-equivalente.png | me-trafo-ensayos (y portada) | 40 kVA, 13 200/231 V, P0 110 W, Pcc 865 W, ucc 4,5 % | me-trafo-equivalente.jpg |
| me-g-paralelo-reparto.png | me-paralelo-transformadores (y portada) | A 100 kVA 4 %, B 50 kVA 5 % | — |
| me-g-trafo-vv-dy11.png | me-paralelo-transformadores | Fasores V-V y Dy11 | me-trafo-trifasico.jpg |
| me-g-cc-dinamos.png | me-maquina-cc | Esquemático | me-cc-curvas-gen.jpg |
| me-g-reaccion-armadura.png | me-maquina-cc | Esquemático | me-cc-reaccion.jpg |
| me-g-cc-motores.png | me-maquina-cc | Derivación 220 V, Ra 0,5 Ω, 40 A, 1500 rpm; serie y compuesto modelados | me-cc-curvas-mot.jpg |
| me-g-ward-leonard.png | me-maquina-cc | Esquemático | me-cc-ward-leonard.jpg |
| me-g-heyland.png | me-motor-asincronico (y portada) | Vacío 380 V 4 A 450 W; bloqueado 76 V 10 A 900 W | — |
| me-g-curvas-v.png | me-maquinas-sincronicas | Xs = 1,74 Ω (Sobrevila, ej. 4.1), 380 V, 30 A | — |
| me-g-cierre-fuera-fase.png | me-maquinas-sincronicas | 2·U·sen(α/2), 380 V | — |
| me-g-alternador-fasores.png | sb-maquina-sincronica (y portada) | Sobrevila, ej. 4.1 | — |
| me-g-asincronico-par-velocidad.png | sb-asincronicos (y portada) | Sobrevila, ej. 5.2–5.3 (20 HP) | — |
| me-g-estrella-triangulo.png | motores-control | Sobrevila, ej. 5.7 | — |
| me-g-trafo50-rendimiento.png | sb-transformadores (y portada) | Sobrevila, ej. 2.3–2.4 | — |
| me-g-trafo40-perdidas.png | me-trafo-rendimiento (y portada) | 40 kVA de la guía de laboratorio | — |
| me-g-rendimiento-calentamiento.png | sb-aspectos-generales (y portada) | Sobrevila, ej. 1.8, 1.9 y 1.10 | — |
| me-g-arranque-reostato.png | sb-cc-especiales (y portada) | Sobrevila, ej. 7.1–7.2; criterio de conmutación propio | — |
| me-g-monofasico-capacitor.png | sb-monofasicos (y portada) | Esquemático | — |
| mat-g-termometro-rampa.png | mat-sistemas-lineales / edo | Ejemplo del artículo (τ = 20 s, 2 °C/min); temperatura inicial tomada | — |
| mat-g-pendientes.png | mat-c1-ecuaciones / separables (y portada) | Apunte de la cátedra, ejemplos de pendiente 2t y decaimiento | — |
| mat-g-senales.png | mat-c2-laplace / tabla (y portada) | Tabla del apunte; constantes tomadas para el dibujo | — |
| mat-g-antitransformadas.png | mat-c3-antitransformada / fracciones (y portada) | Ejemplos del apunte, verificados con SymPy | — |
| mat-g-plano-s.png | mat-c4-sistemas-lineales / polos (y portada) | Ejemplo del apunte; formas del plano esquemáticas | — |
| mat-g-respuesta-impulsiva.png | mat-c5-transferencia / definicion (y portada) | Ejemplo del apunte | — |
| mat-g-segundo-orden.png | mat-c6-mecanicos-electricos / mra (y portada) | Ejemplos de la materia (M-R-A, RLC y masa del apunte) | — |
| mat-g-fourier-cuadrada.png | mat-c7-fourier / serie (y portada) | Ejemplo del apunte (onda cuadrada) | — |
| mat-g-espectro-diesel.png | mat-fourier / transformada | Frecuencias del ejemplo del artículo; amplitudes ilustrativas | — |
| mat-g-armonicos-6p.png | mat-fourier / armonicos | Ejemplo del artículo (rectificador ideal, 1/h) | — |
| mat-g-normal-tolerancia.png | mat-probabilidad / distribuciones | Ejemplo del artículo (ejes del torno, g6) | — |
| mat-g-banera-poisson.png | mat-probabilidad / fallas | Bañera esquemática; Poisson del ejemplo del artículo | — |
| mat-g-confiabilidad.png | mat-c8-probabilidad-militar / mtbf (y portada) | Ejemplos del apunte (p = 0,6; MTBF 5000, 10 000 y 85 000 h) | — |
| mat-g-ajedrez.png | mat-recreativa / ajedrez | Cálculo exacto (2^(n−1)) | — |
| el-g-onda-220.png | el-c3-alterna / valores | Ejemplo del artículo (220 V – 50 Hz) | — |
| el-g-fasor-senoide.png | el-c3-alterna / fasores | Ejemplo del apunte de Ricciuti (10 A, 30°) | — |
| el-g-rlc-serie.png | el-c3-alterna / serie-paralelo (y portada) | Ejemplo del apunte de Ricciuti (R 4, XL 9, XC 6 Ω) | — |
| el-g-rlc-paralelo.png | el-c3-alterna / serie-paralelo | Ejemplo del apunte de Ricciuti (R 5, XL 4, XC 8 Ω) | — |
| el-g-potencia-instantanea.png | el-c4-potencia / instantanea | Ejemplo del artículo (220 V, 10 A, 1000 W) | — |
| el-g-correccion-fp.png | el-c4-potencia / correccion (y portada) | Ejemplo del artículo (iluminación mixta, 0,75 → 0,95) | — |
| el-g-trifasica-fem.png | el-c5-trifasica / ventajas | Red de a bordo de 440 V – 60 Hz | — |
| el-g-campo-rotante.png | el-c5-trifasica / campo | Teorema de Ferraris (por unidad) | — |
| el-g-poliarmonica.png | el-c6-poliarmonicos / parametros (y portada) | Ejemplo del artículo (10 A + 3 A de 5.ª + 2 A de 7.ª); fases nulas para el dibujo | — |
| el-g-electroiman.png | el-c7-ensayos / electroiman (y portada) | Valores ilustrativos (esquema) | — |
| el-g-bobina-real.png | el-c7-ensayos / serie | Datos tomados para el ejemplo | — |
| el-g-cargador-w.png | el-c8-fuentes-cargador / z301 (y portada) | Manual del Z 301-50/302 U (tres puntos unidos con rectas) | — |
| el-g-rectificador-filtro.png | el-c8-fuentes-cargador / convencional | Datos tomados para el ejemplo | — |
| el-g-redes.png | el-c2-redes / mallas (y portada) | Circuitos del apunte de Ricciuti redibujados | — |
| el-g-insercion-voltimetro.png | el-im1-errores-instrumentos / insercion | Ejemplo del artículo (10 V, 50 kΩ) | — |
| el-g-estadistica-lecturas.png | el-im1-errores-instrumentos / estadistica | Ejemplo del artículo (cinco lecturas) | — |
| el-g-corta-larga.png | el-im2-escalas-resistencias / volt-amper | Ejemplo del artículo (RA 0,5 Ω, RV 10 kΩ) | — |
| el-g-aron.png | el-im3-potencia-energia / aron | Ejemplo del artículo (motor de 380 V); corrige el cruce de la lámina | — |
| inst-g-rtd-termistor.png | in-c4-sensores-temperatura / rtd | IEC 60751 (Callendar–Van Dusen), DIN 43760, cobre lineal y NTC con β típico; reemplaza la lámina en inglés repetida en dos artículos | — |
| inst-g-termocuplas.png | in-c4-sensores-temperatura / termocuplas (y portada) | Funciones de referencia NIST ITS-90 (SRD 60) y ejemplo del artículo | — |
| inst-g-tipos-presion.png | in-c3-presion / tipos | Ejemplo del artículo (500 mm Hg de vacío) y manómetro de 3 bar; reemplaza la «Figura 2.1» escaneada | — |
| inst-g-pesas-muertas.png | in-c3-presion / directos | Ejemplo del artículo (10 kg sobre 1 cm²); reemplaza la «Figura 2.7» escaneada | — |
| inst-g-fuelle.png | sensores-medicion / otras | Esquema; reemplaza la lámina en negativo | — |
| inst-g-nonio-calibre.png | in-c2-longitudes / calibre | Lecturas tomadas para el ejemplo (1/20 y 1/50 mm) | — |
| inst-g-nonio-angular.png | in-c2-longitudes / angulos | Lectura del apunte (50°55′); reemplaza la lámina escaneada | — |
| inst-g-mesa-senos.png | in-c2-longitudes / angulos | Ejemplo del artículo (100 mm, 30°) | — |
| inst-g-tolerancia.png | in-c1-metrologia / tolerancias | Ejemplo del apunte (20,5 ± 0,2 mm) | — |
| inst-g-exactitud-precision.png | in-c1-metrologia / errores | Lecturas simuladas (ilustrativo) | — |
| inst-g-pt100-lazo.png | sensores-medicion / ing-pt100 | Ejemplo del artículo, cobre 0,0175 Ω·mm²/m y NAMUR NE 43 | — |
| inst-g-clase-exactitud.png | mediciones-electricas / errores | Ejemplo del artículo (clase 1,5; 250 y 500 V) | — |
| inst-g-shunt-multiplicadora.png | mediciones-electricas / escalas | Ejemplo del artículo (1 mA, 50 Ω) | — |
| inst-g-wheatstone-murray.png | mediciones-electricas / resistencia | Ejemplo del artículo (cable de 300 m) | — |
| mec-g-wohler.png | mc-c1-introduccion / fatiga (portada) | Shigley: Se' = 0,5·Sut, 0,9·Sut a 10³ ciclos; acero de ejemplo de 600 MPa | — |
| mec-g-union-abulonada.png | mc-c2-uniones-abulonadas / verificacion (portada) | Bulón de ¼″ del artículo; rigidez de las piezas supuesta | — |
| mec-g-pielstick-velocidad.png | mc-c3-biela-manivela / dinamica (portada) | Pielstick 16 PC2-5 del artículo (r 230, L 955 mm) | mc-pielstick-velocidad.jpg |
| mec-g-biela-fuerzas.png | mc-c3-biela-manivela / fuerzas | Fórmulas del artículo, λ = 0,241, α = 40° | mc-biela-fuerzas.jpg |
| mec-g-engranajes-relaciones.png | mc-c4-engranajes / basico (portada) | Ejemplos del artículo (módulo 5; tren de 150 CV) | mc-engranajes-relaciones.jpg |
| mec-g-engranajes-fuerzas.png | mc-c4-engranajes / basico | Par de módulo 5, 10 CV a 1200 rpm, φ = 20° | mc-engranajes-fuerzas.jpg |
| mec-g-desalineaciones.png | mc-c6-acoplamientos-vibraciones / alineacion | Esquema propio | mc-desalineaciones.jpg y alineacion-acoplamientos-metodos-1.jpg (repetidas) |
| mec-g-tolerancias-alineacion.png | mc-c6-acoplamientos-vibraciones / alineacion | Tabla de tolerancias de la clase | alineacion-acoplamientos-metodos-4.jpg |
| mec-g-borde-cara.png | mc-c6-acoplamientos-vibraciones / alineacion | Lecturas tomadas para el ejemplo | mc-comparadores.jpg |
| mec-g-stribeck.png | mc-c5-cojinetes / friccion | Forma cualitativa | mc-tower.jpg |
| mec-g-amplificacion.png | mc-c6-acoplamientos-vibraciones / vibraciones | Rotor de TG del artículo (0,10 mm de flecha) | — |
| hn-g-precarga-acumulador.png | hn-c1-oleohidraulica / acumuladores | Datos tomados (10 L, 100–200 bar, p0 90 y 45 bar) | hn-recarga-acumulador.jpg (y el cuadro hn-acumuladores-resumen.jpg, ya en tabla) |
| hn-g-triangulos.png | hn-c2-centrifugas / ecuaciones | Rodete tomado (Ø 250 mm, 1450 rpm, β2 25°) | hn-triangulos-velocidad.jpg |
| hn-g-curvas-centrifuga.png | hn-c2-centrifugas / curvas | Bomba tomada; leyes de semejanza del artículo | hn-curvas-centrifuga.jpg |
| hn-g-punto-funcionamiento.png | hn-c3-instalacion / punto (portada) | Bomba e instalación tomadas | hn-punto-funcionamiento.jpg |
| hn-g-bombas-paralelo.png | hn-c3-instalacion / regulacion | Ídem | hn-bombas-paralelo.jpg |
| hn-g-bombas-serie.png | hn-c3-instalacion / regulacion | Ídem | hn-bombas-serie.jpg |
| hn-g-anpa.png | hn-c4-cavitacion / anpa | Ejemplo del artículo (curvas esquemáticas) | hn-anpa-zonas.jpg y hn-ejemplo-anpa.jpg |
| hn-g-beta.png | hn-c5-contaminacion / filtros (portada) | η = 1 − 1/β; ejemplo del artículo | hn-beta.jpg (y hn-iso-rangos.jpg, ya en tabla) |
| hn-g-reynolds-flushing.png | hn-c5-contaminacion / flushing | Ejemplo del artículo; ISO VG 32 por ASTM D341 | hn-flushing-reynolds.jpg |
| eo-g-diodo-aproximaciones.png | eo-c1-diodos / tipos (y portada) | Ejemplo del artículo (12 V, 2,2 kΩ) y curva de Shockley con parámetros típicos; reemplaza dos láminas | — |
| eo-g-rectificadores.png | eo-c2-rectificadores / bloques; portada de electronica-analogica | Ejemplo del artículo (24 V eficaces, 470 Ω); reemplaza dos láminas dibujadas a mano | — |
| eo-g-filtro-rizado.png | eo-c2-rectificadores / filtro | Ejemplo del artículo (100 mA, 1000 µF, 50 Hz), simulado; reemplaza la lámina dibujada a mano | — |
| eo-g-zener.png | eo-c2-rectificadores / filtro | Ejemplo del artículo (20 V, 470 Ω, Zener 12 V) | — |
| eo-g-recta-carga-bjt.png | eo-c3-transistor / divisor (y portada) | Ejemplo 3 del apunte; curvas esquemáticas | — |
| eo-g-bc337-beta.png | eo-c3-transistor / divisor | Ejemplo del artículo (BC337, β 100 a 630) | — |
| eo-g-operacionales.png | eo-c4-operacionales / configuraciones (y portada) | Ejemplos del artículo | — |
| eo-g-transferencia-op.png | eo-c4-operacionales / configuraciones | Ejemplos del artículo; saturación típica ±13 V supuesta | — |
| eo-g-cmrr.png | electronica-analogica / operacional | Ejemplo del artículo (Vd 50 µV, Vc 125 µV, Ad 5000) | — |
| eo-g-compuertas.png | eo-c5-digital / boole | Tablas generadas por código; reemplaza la lámina de la AND | — |
| eo-g-logica-problemas.png | eo-c5-digital / problemas | Soluciones del artículo, comprobadas por código | — |
| eo-g-cuantizacion.png | electronica-digital / conversores (y portada) | Ejemplo del artículo (0–10 bar, 4–20 mA) | — |
| ha-g-aleta-sustentacion.png | estabilizadores-rolido / cat-teoria-estab | Aleta del MEKO 360 (25,7 t a 25°); desprendimiento esquemático | ha-est-ruido.jpg |
| ha-g-timon-joessel.png | gobierno-timon / cat-gob-teoria | Fórmulas de Joessel; pala de ejemplo | ha-gob-circulo.jpg |
| ha-g-gobierno-m360.png | gobierno-timon / cat-gob-m360 | Hoja técnica de la R4S 380 | gob-m360-configuracion.jpg (manuscrita) |
| ha-g-hpc-empuje.png | helice-paso-controlable / comportamiento | Serie B de Wageningen; hélice de ejemplo; resistencia esquemática | helice-paso-controlable-comportamiento-2.jpg |
| ha-g-indice-viscosidad.png | ha-liquidos-hidraulicos / indice-viscosidad (portada) | ASTM D341, valores tomados | ha-liq-iv.jpg |
| sp2-g-libertad-potencia.png | sp-analisis-sistemas (portada) | Libertad 2 × 960 kW a 13,7 kn; Np ∝ Vs³, S ∝ Vs² | interactivo sim-helice repetido |
| sp2-g-remolque.png | sp-analisis-sistemas / remolque | Libertad; K × 2,5 supuesto | sp2-oga-remolque.jpg |
| sp2-g-droop.png | sp-analisis-sistemas / plantas | definición de droop, 60 Hz | sp2-oga-droop.jpg |
| sp2-g-waterjet-rendimiento.png | waterjet / allison-teoria | fórmula de Allison (1993) | wj-allison-rendimiento.jpg |
| sp2-g-evolucion-gas.png | g30-turbina-ciclos / principio | ciclo Brayton calculado (relación 12, 1350 K) | tg/evolucion-gas.jpg y g30-turbina-ciclos-principio-1.jpg |
| sp2-g-aire-camara.png | g31-turbina-organos / camara | porcentajes de la lámina de la cátedra | tg/distribucion-aire-camara.jpg y g31-turbina-organos-camara-1.jpg |
| sp2-g-compresores.png | g31-turbina-organos / centrifugo | esquema cualitativo | tg/compresor-centrifugo.jpg, g31-turbina-organos-centrifugo-2.jpg y axial-2.jpg |
| ctl-g-franja-error.png | ctl-c3-requisitos / transitorio | segundo orden calculado (ωn = 1 rad/s, ζ ilustrativos) | ctl-franja-error.jpg |
| ctl-g-transitoria.png | ctl-c4-respuesta-temporal / especificaciones (portada) | ζ = 0,5, ωn = 4 rad/s del artículo | ctl-transitoria-parametros.jpg |
| ctl-g-primer-orden-rampa.png | ctl-c4-respuesta-temporal / primer-orden | termómetro T = 12 s del artículo | — |
| ctl-g-polos.png | ctl-c2-modelado / propiedades; portada de mat-sistemas-lineales | H1 y H2 del apunte (SymPy) | — |
| ctl-g-tanque.png | ctl-c2-modelado / linealizacion | tanque del artículo (A 2 m², h 1,2 m, a 0,01 m²) | — |
| ctl-g-dos-posiciones.png | ctl-c5-acciones / si-no | tanque y caudales ilustrativos | ctl-nivel-dos-posiciones.jpg |
| ctl-g-p-pi-pid.png | ctl-c5-acciones / pid (portada) | planta 1/(s + 1)³ y ajustes ilustrativos | ctl-integral-sobrecorrige.jpg |
| ctl-g-sintonia-pi.png | sistemas-control / ing-sintonia (portada) | K 2, θ 10 s, τ 60 s del artículo | — |
| ctl-g-bode-primer-orden.png | ctl-c6-frecuencia / bode | 1/(1 + jωT) | ctl-bode-primer-orden.jpg (mal rotulada) |
| ctl-g-bode-servo.png | ctl-c6-frecuencia / bode (portada) | 10/[s(1 + 0,5s)] del artículo | — |
| ctl-g-escalera.png | ctl-escalera / escalera (portada) | escalera simulada por código | — |
| ctl-g-semaforo.png | ctl-reles-programables / practicas | práctica 5c del curso de LOGO! | — |
| ctl-g-scan.png | plc / ing-scan (portada) | 600 rpm y scan de 20 ms del artículo | — |
| an-g-francobordo.png | an-c1-definiciones / dimensiones (portada) | Convenio de Líneas de Carga 1966 (separaciones ilustrativas) | an-plimsoll.jpg |
| an-g-coeficientes.png | an-c1-definiciones / coeficientes | ejemplo del artículo (L 100, B 15, T 5 m) | — |
| an-g-metacentro.png | an-c2-estabilidad-inicial / metacentro (portada) | pontón propio de 60 × 12 × 6 m | an-metacentro.jpg |
| an-g-bloque.png | an-c2-estabilidad-inicial / equilibrio | bloque de madera del artículo | — |
| an-g-superficie-libre.png | an-c3-superficies-libres / superficies (portada) | tanque de 10 m, Δ 3500 t (Barrass) | — |
| an-g-inclinacion.png | an-c3-superficies-libres / inclinacion | buque del ejemplo, lecturas propias | — |
| an-g-curva-gz.png | an-c4-grandes-angulos / cruzadas (portada) | pontón propio, G en crujía y a 0,36 m | an-escora-permanente.jpg |
| an-g-loll.png | an-c4-grandes-angulos / negativo | pontón propio con KG 5,7 m | — |
| an-g-asiento.png | an-c5-longitudinal-dinamica / longitudinal | buque N-N del artículo (8200 t) | an-variacion-calados.jpg |
| an-g-viento.png | an-c5-longitudinal-dinamica / dinamica | esquema | an-viento.jpg |
| an-g-estabilidad-dinamica.png | an-c5-longitudinal-dinamica / dinamica (portada) | pontón propio, brazo de viento ilustrativo | an-estabilidad-dinamica.jpg |
| an-g-criterios-is.png | estabilidad-buque / criterios | pontón propio y Código IS 2008 | — |
| tm-g-ajustes.png | tm-c1-ajustes / definiciones (portada) | ejemplos del artículo e ISO 286-2 | tm-ajuste-casos-juego.jpg |
| tm-g-calidades-it.png | tm-c1-ajustes / sistema-iso | ISO 286-1 (30–50 mm) | tm-calidades-it.jpg |
| tm-g-posiciones.png | tm-c1-ajustes / sistema-iso | ISO 286-2 (50 mm) | tm-agujero-unico.jpg, tm-eje-unico.jpg |
| tm-g-montaje.png | tm-c1-ajustes / montaje | ejemplo del artículo (120 h6/R7) | — |
| tm-g-defectos-forma.png | tm-c2-verificacion / defectos | esquema | tm-defecto-circularidad.jpg, tm-defecto-cilindricidad.jpg |
| tm-g-ra-rz.png | tm-c3-rugosidad / parametros (portada) | perfil ilustrativo, ISO 4287 | tm-rugosidad-ra.jpg, tm-rugosidad-rz.jpg |
| tm-g-rugosidad-procesos.png | tm-c3-rugosidad / aplicaciones | lámina de la cátedra | tm-rugosidad-procesos.jpg |
| tm-g-micrometro.png | tm-c4-calibres-micrometros / micrometro | ejemplo del artículo (7,73 mm) | tm-tornillo-micrometrico.jpg |
| tm-g-calas.png | tm-c5-comparadores / calas | ejemplo del artículo (99,995 mm) | — |
| tm-g-medicion-indirecta.png | tm-c5-comparadores / directa-indirecta | ejemplo del artículo | tm-medicion-indirecta.jpg |
| tm-g-juego-dientes.png | tm-c6-cajas-reductoras / juegos | ejemplo del artículo (m 5, a 1000 mm) | — |
| tm-g-regimenes-engranajes.png | tm-c7-fallas / engranajes | esquema cualitativo | tm-regimenes-engranajes.jpg |
| tm-g-scania-di13.png | tm-c8-scania-di13 / curvas (portada) | hoja de datos Scania DI13 078M | — |
| met-g-traccion.png | met-c2-ensayos-mecanicos / traccion (portada) | curva ilustrativa con los mínimos GL | met-c2-06.jpg |
| met-g-celdas.png | met-c3-estructura / celdas | esquema calculado | met-c3-04.jpg, met-c3-05.jpg |
| met-g-trefilado.png | met-c4-trabajado-recocido / acritud | ejemplo del artículo | — |
| met-g-recocido.png | met-c4-trabajado-recocido / recocido (portada) | esquema cualitativo | met-c4-25.jpg |
| met-g-palanca-cuni.png | met-c5-soluciones-solidas / interpretacion | ejemplo del artículo | — |
| met-g-palanca-pbsn.png | met-c6-eutecticos-aluminio / eutectico | ejemplo del artículo | — |
| met-g-enfriamiento-hierro.png | met-c7-aceros-fundiciones / hierro | temperaturas del hierro puro | met-c7-02.jpg |
| met-g-fe-fe3c.png | met-c7-aceros-fundiciones / diagrama (portada) | puntos del artículo | met-c7-05.jpg |
| met-g-fases-acero.png | met-c7-aceros-fundiciones / aceros | regla de la palanca del artículo | — |
| met-g-tratamientos.png | met-c8-tratamientos / recocidos | reglas de la tabla del artículo | met-c8-18.jpg, met-c8-24.jpg |
| ta-g-ph-r22.png | ta-conceptos-refrigeracion / ciclo | ejemplo de 25 000 frig/h con CoolProp (R22) | ta-tema1-17.jpg |
| ta-g-presiones.png | ta-conceptos-refrigeracion / presion | presiones de saturación de CoolProp | ta-tema1-2.jpg |
| ta-g-evaporador.png | ta-evaporadores / enfriadores-aire | ejemplo de la cámara de −20 °C | ta-tema2-6.jpg |
| ta-g-condensador.png | ta-condensadores / aire | ejemplo agua de mar contra aire con CoolProp | — |
| ta-g-relacion-compresion.png | ta-compresores-frigorificos / alternativos | ciclo ideal del R22 con CoolProp | — |
| ta-g-recalentamiento.png | ta-controles-refrigeracion / vet | rango de 5–7 °C del apunte (esquemático) | ta-tema5-17.jpg |
| ta-g-psicrometria.png | aire-acondicionado / aire-humedo | valores de la calculadora; aire húmedo de CoolProp | — |
| ta-g-tobera.png | toberas-eyectores / critica | relaciones isentrópicas | — |
| ta-g-ebullicion.png | destiladores / vacio | saturación del agua de CoolProp | — |
| ta-g-dtml.png | intercambiadores / calculo | ejemplo ilustrativo | — |
| se2-g-caida-arranque.png | planta-electrica / ing-arranque-motor | ejemplo del artículo | — |
| se2-g-cadena.png | propulsion-electrica / ing-cadena | ejemplo del artículo | — |
| se2-g-armonicos.png | propulsion-electrica / convertidores | rectificador ideal | — |
| se2-g-coordinacion.png | protecciones-electricas / ing-coordinacion | ejemplo del artículo (IEC normal inversa) | — |
| se2-g-error-giro.png | girocompas-correderas / ing-error-velocidad | fórmula del artículo | — |
| se2-g-corredera.png | girocompas-correderas / correderas | OMI MSC.96(72) | — |
| lci-g-ramas.png | lci-proteccion / ramas | esquema propio (curso de LCI, SOLAS II-2) | — |
| lci-g-tetraedro.png | lci-quimica / tetraedro | esquema propio | — |
| lci-g-inflamabilidad.png | lci-quimica / mezcla | ICSC 1561, JRC | — |
| lci-g-oxigeno.png | lci-quimica / elementos | curso de LCI, OSHA 29 CFR 1910.146 | — |
| lci-g-fases.png | lci-calor / fases | curso de LCI (esquemático) | — |
| lci-g-agua.png | lci-agentes / agua | CoolProp | — |
| lci-g-espuma.png | lci-agentes / espuma | curso de LCI, NFPA 11 | — |
| lci-g-conexion.png | lci-extintores / conexion | Código SSCI cap. 2 | — |
| lci-g-co2.png | lci-sala-maquinas / fijos | Código SSCI cap. 5, NIOSH | — |
