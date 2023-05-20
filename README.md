# proyecto-final
//@name <makeStruct>
//@param <moto, char> 
//@param <csvString,char>
//@return <nanais de paraguais>
void makeStruct(Moto *moto, char *csvString) {
    char *token = strtok(csvString, ",");

    // Asignar valores a la estructura de la moto
    moto->nombrePropietario = strdup(token);

    token = strtok(NULL, ",");
    moto->apellidoPropietario = strdup(token);

    token = strtok(NULL, ",");
    moto->placa = strdup(token);

    token = strtok(NULL, ",");
    moto->horaEntrada = strdup(token);
}

