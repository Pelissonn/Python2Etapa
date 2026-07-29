Windows PowerShell
Copyright (C) Microsoft Corporation. Todos os direitos reservados.

PS C:\Users\12402184> Invoke-RestMethod http://127.0.0.1:5000/api/livros `
>>    -Method POST `
>>    -ContentType "application/json" `
>>    -Body '{"titulo":"O T triplo","autor":"Coelho","ano":1867}'


ano          : 1867
autor        : Coelho
data_criacao : 2026-07-29 08:58:32.991321
id           : 4
titulo       : O T triplo



PS C:\Users\12402184> Invoke-RestMethod http://127.0.0.1:5000/api/livros `
>>    -Method POST `
>>    -ContentType "application/json" `
>>    -Body '{"titulo":"NOME DO LIVRO","autor":"NOME DO AUTOR","ano":ANO DA PUBLICAÇÃO}'
Invoke-RestMethod :
400 Bad Request
Bad Request
Failed to decode JSON object: &#39;utf-8&#39; codec can&#39;t decode byte 0xc7 in position 70: invalid continuation
byte
No linha:1 caractere:1
+ Invoke-RestMethod http://127.0.0.1:5000/api/livros `
+ ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
    + CategoryInfo          : InvalidOperation: (System.Net.HttpWebRequest:HttpWebRequest) [Invoke-RestMethod], WebExc
   eption
    + FullyQualifiedErrorId : WebCmdletWebResponseException,Microsoft.PowerShell.Commands.InvokeRestMethodCommand
PS C:\Users\12402184> Invoke-RestMethod http://127.0.0.1:5000/api/livros `
>>    -Method POST `
>>    -ContentType "application/json" `
>>    -Body '{"titulo":"Elementos","autor":"Euclides de Alexandria","ano":300}'


ano          : 300
autor        : Euclides de Alexandria
data_criacao : 2026-07-29 09:04:19.593642
id           : 5
titulo       : Elementos



PS C:\Users\12402184> Invoke-RestMethod http://127.0.0.1:5000/api/livros `
>>    -Method POST `
>>    -ContentType "application/json" `
>>    -Body '{"titulo":"O Homem que calculava","autor":"Malba Tahan","ano":1928}'


ano          : 1928
autor        : Malba Tahan
data_criacao : 2026-07-29 09:05:32.631162
id           : 6
titulo       : O Homem que calculava



PS C:\Users\12402184> Invoke-RestMethod http://127.0.0.1:5000/api/livros `
>>    -Method POST `
>>    -ContentType "application/json" `
>>    -Body '{"titulo":"O que é matematica","autor":"Richard Courant & Herbert Robbins","ano":1941}'
Invoke-RestMethod :
400 Bad Request
Bad Request
Failed to decode JSON object: &#39;utf-8&#39; codec can&#39;t decode byte 0xe9 in position 17: invalid continuation
byte
No linha:1 caractere:1
+ Invoke-RestMethod http://127.0.0.1:5000/api/livros `
+ ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
    + CategoryInfo          : InvalidOperation: (System.Net.HttpWebRequest:HttpWebRequest) [Invoke-RestMethod], WebExc
   eption
    + FullyQualifiedErrorId : WebCmdletWebResponseException,Microsoft.PowerShell.Commands.InvokeRestMethodCommand
PS C:\Users\12402184> Invoke-RestMethod http://127.0.0.1:5000/api/livros `
>>    -Method POST `
>>    -ContentType "application/json" `
>>    -Body '{"titulo":"O que e matematica","autor":"Richard Courant e Herbert Robbins","ano":1941}'


ano          : 1941
autor        : Richard Courant e Herbert Robbins
data_criacao : 2026-07-29 09:07:54.076380
id           : 7
titulo       : O que e matematica



PS C:\Users\12402184> Invoke-RestMethod http://127.0.0.1:5000/api/livros `
>>    -Method POST `
>>    -ContentType "application/json" `
>>    -Body '{"titulo":"A arte de resolver","autor":"George Polya","ano":1945}'


ano          : 1945
autor        : George Polya
data_criacao : 2026-07-29 09:10:24.278050
id           : 8
titulo       : A arte de resolver



PS C:\Users\12402184> Invoke-RestMethod http://127.0.0.1:5000/api/livros `
>>    -Method POST `
>>    -ContentType "application/json" `
>>    -Body '{"titulo":"Fundamentos de matematica elementar","autor":"gelson lezzi e carlos murakami","ano":1977}'


ano          : 1977
autor        : gelson lezzi e carlos murakami
data_criacao : 2026-07-29 09:11:53.082194
id           : 9
titulo       : Fundamentos de matematica elementar



PS C:\Users\12402184> Invoke-RestMethod http://127.0.0.1:5000/api/livros `
>>    -Method POST `
>>    -ContentType "application/json" `
>>    -Body '{"titulo":"O ultimo teorema de fermat","autor":"Simon singh","ano":1997}'


ano          : 1997
autor        : Simon singh
data_criacao : 2026-07-29 09:12:45.101582
id           : 10
titulo       : O ultimo teorema de fermat



PS C:\Users\12402184> Invoke-RestMethod http://127.0.0.1:5000/api/livros `
>>    -Method POST `
>>    -ContentType "application/json" `
>>    -Body '{"titulo":"O livro da matematica","autor":"Dorling Kindersley","ano":2012}'


ano          : 2012
autor        : Dorling Kindersley
data_criacao : 2026-07-29 09:13:39.521684
id           : 11
titulo       : O livro da matematica



PS C:\Users\12402184> Invoke-RestMethod http://127.0.0.1:5000/api/livros `
>>    -Method POST `
>>    -ContentType "application/json" `
>>    -Body '{"titulo":"The joy of x","autor":"steven strogatz","ano":2012}'


ano          : 2012
autor        : steven strogatz
data_criacao : 2026-07-29 09:14:23.703551
id           : 12
titulo       : The joy of x



PS C:\Users\12402184> Invoke-RestMethod http://127.0.0.1:5000/api/livros `
>>    -Method POST `
>>    -ContentType "application/json" `
>>    -Body '{"titulo":"how to not be wrong","autor":"jordan ellenberg","ano":2014}'


ano          : 2014
autor        : jordan ellenberg
data_criacao : 2026-07-29 09:15:05.835250
id           : 13
titulo       : how to not be wrong



PS C:\Users\12402184> Invoke-RestMethod http://127.0.0.1:5000/api/livros/1 `
>>    -Method PUT `
>>    -ContentType "application/json" `
>>    -Body '{"titulo":"Cotemig","autor":"3A1","ano":2026}'


ano          : 2026
autor        : 3A1
data_criacao : 2026-07-29 08:51:09.709106
id           : 1
titulo       : Cotemig


PS C:\Users\12402184> Invoke-RestMethod http://127.0.0.1:5000/api/livros/5 -Method DELETE

PS C:\Users\12402184> Invoke-RestMethod http://127.0.0.1:5000/api/livros/6 -Method DELETE

PS C:\Users\12402184> Invoke-RestMethod http://127.0.0.1:5000/api/livros/7 -Method DELETE

PS C:\Users\12402184>