# MovMul-S2

class Alumno {
  String? nombres;
  String? apellidos;
  int? nota1;
  int? nota2;
  int? nota3;
  
  Alumno.nombre(this.nombres, this.apellidos);
  Alumno.notas(this.nota1, this.nota2, this.nota3);
  
  @override
  String toString() {
    return 'Nombre Completo: $nombres, $apellidos'; // 
  }
  
  String notas(){
    return 'Nota1: $nota1 Nota2: $nota2 Nota3: $nota3';
  }
}


void main() {
  final andres = Alumno.nombre("Andres", "Huancahuari");
  andres.nota1 = 15;
  andres.nota2 = 19;
  andres.nota3 = 16;
  final alex = Alumno.notas(17,18,18);
  alex.nombres = "Alex";
  alex.apellidos = "HQ";
  
  print(andres.nombres);
  print(andres.nota1);
  print(andres.nota2);
   print(andres.nota3);
  print(andres.toString());
  print(alex.notas());
  print(alex.toString());
  
}
