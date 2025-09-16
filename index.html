from machine import Pin, ADC
import time

print("Iniciando ESP32 - Controle de LEDs por LDR")

# --- Configuração do pino do LDR ---
PINO_LDR = 4
sensor_ldr = ADC(Pin(PINO_LDR))
sensor_ldr.width(ADC.WIDTH_12BIT)   # resolução 12 bits (0..4095)
sensor_ldr.atten(ADC.ATTN_11DB)     # faixa de tensão até 3.3V

# --- Configuração dos LEDs ---
PINO_LED1 = 19   # LED1 - acende quando escuro
PINO_LED2 = 23   # LED2 - acende quando claro
led1 = Pin(PINO_LED1, Pin.OUT)
led2 = Pin(PINO_LED2, Pin.OUT)

# --- Limiares de luminosidade ---
LIMIAR_ESCURO = 2000   # abaixo disso → LED1 acende
LIMIAR_CLARO = 2000    # acima disso → LED2 acende

# --- Loop principal ---
while True:
    valor_luminosidade = sensor_ldr.read()
    print("Valor de luminosidade:", valor_luminosidade)

    if valor_luminosidade < LIMIAR_ESCURO:
        # Pouca luz → LED1 ligado
        led1.on()
        led2.off()
        print("Ambiente escuro → LED1 ligado, LED2 desligado")

    else:
        # Muita luz → LED2 ligado
        led1.off()
        led2.on()
        print("Ambiente claro → LED2 ligado, LED1 desligado")

    time.sleep(1)
