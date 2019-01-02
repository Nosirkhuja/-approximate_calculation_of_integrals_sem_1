const
  n = 10;

var
  mass: array[1..n] of integer;
  p, k, i: integer;

begin
  for i := 1 to n do read(mass[i]); 
  if n < 2 then begin write('NO');exit; end; 
  p := mass[2];   
  if n < 4 then begin write('YES');exit; end;
  if n >= 4 then begin
    if mass[2] > mass[4] then k := 1
    else k := 2; end;
  if k = 1 then begin
    for i := 3 to n do 
    begin
      if (not odd(i)) then begin
        if p > mass[i] then p := mass[i]
        else begin write('NO');exit end; end; end; end;
  if k = 2 then begin
    for i := 3 to n do 
    begin
      if (not odd(i)) then begin
        if p <= mass[i] then p := mass[i]
        else begin write('NO');exit end; end; end; end; 
  write('YES');
end.
