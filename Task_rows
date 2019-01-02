var
  i,j,k,m:integer;
  s,t:string;
  a:array[1..128] of string;{массив уникальных слов}
  n:array[1..128] of integer;{количество повторов каждого слова}
procedure additem;{довавляем слово или увеличиваем счетчик повторов}
var
  k:integer;
begin
  if t<>'' then
  for k:=1 to j do if a[k]=t then begin{слово есть в списке - увеличиваем счетчик}
    n[k]:=n[k]+1;
    if n[m]<n[k] then m:=k;{заодно запоминаем индекс с максимальным числом повторов}
    t:='';
    break;
  end;
  if t<>'' then begin{слова в списке нет, добавляем}
   j:=j+1;
   n[j]:=1;
   a[j]:=t;
   t:=''
  end;
end;
begin
  i:=0;j:=0;m:=1; t:='';
  write('CTPOKA:'); readln(s);
  for i:=1 to length(s) do if s[i]<>' ' then t:=t+s[i] else additem;{разбираем на слова}
  additem;{не забывем про последнее слово}
  for i:=1 to j do begin
    if n[i]=n[m] then writeln(a[i]);{печатаем все слова равные количеству максимальных повторов}
  end;
end.
