var
  a, b: real;
  m: integer;

function integral_(var a, b: real): real;{https://ru.wikipedia.org/wiki/Формула_Симпсона}
var
  c: real;
begin
  Write('Верхний предел: ');
  Readln(a);
  Write('Нижний предел: ');
  Readln(b);
  c := (a + b) / 2; 
  integral_ := (((b - a) / 6) * (-2 * a * a * a - 20 * a * a - 55 * a - 1709 + 4 * (-2 * c * c * c - 20 * c * c - 55 * c - 1709) + -2 * b * b * b - 20 * b * b - 55 * b - 1709));
end;

function error_(a, b: real): real;{http://www.cleverstudents.ru/integral/method_of_trapezoids.html#assessment_of_error}
begin
  Write('Верхний предел: ');
  Readln(a);
  Write('Нижний предел: ');
  Readln(b); 
  error_ := (12 * b - 40) * (b - a) * (b - a) * (b - a) / (12 * 3 * 3);
end;

begin
  writeln('0 - выход из программы');
  writeln('1 - Ввод пределов интегрирования');
  writeln('2 - Оценка погрешности');
  readln(m);
  case m of 
    0: exit; 
    1: begin write(integral_(a, b))end; 
    2: begin write(error_(a, b)) end; 
  end;
end.
