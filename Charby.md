```c#
using System;

namespace readd

{

class Program

{

static void Main(string[] args)

{

Console.WriteLine("Ingrese su nombre");

string name = Console.ReadLine();

if(typeCheckInt(name)== true)

{

Console.WriteLine("No ingrese numeros");

return;

}

else

{

Console.WriteLine("Bienvenido" + name);

}

Console.WriteLine("Ingrese su apellido");

string lastname = Console.ReadLine();

if(typeCheckInt(lastname)== true)

{

Console.WriteLine("No ingrese numeros");

return;

}

else

{

Console.WriteLine(name + " "  + lastname);

}

try

{

Console.WriteLine("Ingrese su edad");

int age = int.Parse(Console.ReadLine());

Console.WriteLine("Ingrese su cedula");

int cedula = int.Parse(Console.ReadLine());

}

catch(Exception error)

{

Console.WriteLine("No ingrese letras solo numeros" + error.Message);

}

Console.WriteLine("Ingrese Password");

string password = Console.ReadLine();

Console.WriteLine("Confirme Password");

string confirmPassword = Console.ReadLine();

if(confirmPassword == password)

{

Console.WriteLine("Verificada");

}

else

{

Console.WriteLine("El Password no es igual");

}

}

static bool typeCheckInt(string input)

{

int number = 0;

return int.TryParse(input,out number);

}

}

}

Console.WriteLine("Ingrese su password");

string Password = Console.ReadLine();

Console.WriteLine("Confirme su password");

string confirmPassword = Console.ReadLine();

if (Password != confirmPassword)

{

Console.WriteLine("No es la misma Password");

return;

}

else

Console.WriteLine("Verificada");

}

static bool typeCheckInt(String input)

{

int number = 0;

return int.TryParse(input,out number);

}

}

}
```