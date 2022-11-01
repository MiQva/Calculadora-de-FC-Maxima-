# Calculadora-de-frecuencia-cardiaca-máxima-teórica

sexo = int(input('Escriba 1 si es hombre y 2 si es mujer: '))

if sexo != 1 and sexo != 2:
    print('¡Error, introduce las credenciales correctamente!')
    exit()

deportista = str(input('Escriba si es deportista (si o no): '))

if deportista != 'si' and deportista != 'no':
    print('¡Error, introduce las credenciales correctamente!')
    exit()

edad = int(input('Por ultimo escriba su edad de forma numerica: '))

if edad > 100 and edad < 0:
    print('¡Error, introduce las credenciales correctamente!')

if sexo == 1 and deportista == 'no':
    frequencia_1 = str(220 - edad)
    print('Su frecuencia cardiaca máxima es de '+ frequencia_1)
elif sexo == 1 and deportista == 'si':
    frequencia_2 = str(208 - (0.7 * edad))
    print('Su frecuencia cardiaca máxima es de '+ frequencia_2)

if sexo == 2 and deportista == 'no':
    frequencia_1 = str(226 - edad)
    print('Su frecuencia cardiaca máxima es de '+ frequencia_1)
elif sexo == 2 and deportista == 'si':
    frequencia_3 = str(214 - (0.8 * edad))
    print('Su frecuencia cardiaca máxima es de '+ frequencia_3)
