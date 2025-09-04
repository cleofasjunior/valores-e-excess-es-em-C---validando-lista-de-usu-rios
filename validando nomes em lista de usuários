using System;
using System.Collections.Generic;
using System.Linq;

class Program
{
    static void Main()
    {
        string inputLine = Console.ReadLine();

        var names = inputLine.Split(',')
                               .Select(n => n.Trim().Trim('"'))
                               .ToList();

        var validNames = new List<string>();
        var errors = new List<string>();

        foreach (var name in names)
        {
            if (name == "null")
            {
                errors.Add("Erro: nome nulo");
            }
            else if (string.IsNullOrWhiteSpace(name))
            {
                errors.Add("Erro: nome invalido");
            }
            else
            {
                validNames.Add(name);
            }
        }

        if (errors.Any())
        {
            string validosString = string.Join(", ", validNames);
            string errosString = string.Join(" / ", errors);

            if (string.IsNullOrWhiteSpace(validosString))
            {
                Console.WriteLine(errosString);
            }
            else
            {
                Console.WriteLine($"{validosString} / {errosString}");
            }
        }
        else
        {
            Console.WriteLine(string.Join(", ", validNames));
        }
    }
}
