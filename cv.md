# Gorlov Nikita

## Contacts
* E-mail: Nik-NameG@rambler.ru
* GitHub: [NikitoLa](https://github.com/NikitoLa)
* rs-school discord nickname: glomer(@NikitoLa)

## About me
I'm third-year student of SUAI (State University of Aerospace Instrumentation). I study applied mathematics and computer science. Also in my spare time i do self-education, watch science-popular videos and read what is happening in the world. I have tried myself at various jobs, but they are not related to the IT sphere. i'm pretty keen on challenging myself with different task and complete them (can spend hours solving interesting coding or math problem). I'd like to see myself as a developer in company solving really interesting problems

## Skills

1. Git/GitHub
2. C++ (basics, OOP, multithreading). C++ framework: Qt
3. HTML5/CSS3
4. JS basics
5. Windows OS, Linux(Ubuntu)

## Code example

[some algorithms and data structures](https://github.com/NikitoLa/structures-and-algorithms)

function on C++ that converts Int32 to IPv4
```
#include <cmath>
std::string uint32_to_ip(uint32_t ip)
{
  std::string str_ip = "";
  std::string res = "";
  int remains;
    
  while (ip != 0 )
  {
    remains = ip % 2;
    ip /= 2;
    str_ip = std::to_string(remains) + str_ip;
  }
  
  for (str_ip.size(); str_ip.size() < 32; )
  {
    str_ip = "0" + str_ip;  
  }
  
  for (int i = 0; i < 4; i++)
  {
    int index = i * 8;
    int sum = 0;
    
    for (int j = 0; j < 8; j++)
    {
      sum += int(str_ip[index] - '0') * std::pow(2, 7 - j);
      index++;
    }
    
    res += std::to_string(sum);
    if (index < 30)
    {
      res += '.';
    }
  }
  return res;
}
```

## Education and cources

* Bachelor, SUAI, St.Petesburg
* RS-school JavaScript/Front-end 2023Q1 (in process)
