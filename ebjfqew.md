代发 wailian999

Ruby: PI = 3.14159
来源：https://bw.zhonguo2118.cn

C#:   const double PI = 3.14159;
来源：https://mi.zhonguo4118.cn

[A04] 判断变量类型
来源：https://rx.zhonguo3118.cn

Py:   type(x).__name__; isinstance(x, int)
来源：https://wj.zhonguo2118.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：https://gd.zhonguo4118.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：https://ri.zhonguo6118.cn

TS:   typeof x; x instanceof Date
来源：https://eq.zhonguo1118.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：https://dd.zhonguo5118.cn

Go:   reflect.TypeOf(x).Name()
来源：https://um.zhonguo8118.cn

Ruby: x.class; x.is_a?(Integer)
来源：https://ec.zhonguo2118.cn

C#:   x.GetType().Name; x is int
来源：https://qv.zhonguo7118.cn

[A05] 整数除法与取模
来源：https://tn.zhonguo6118.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：https://df.zhonguo8118.cn

PHP:  intdiv(7, 2); 7 % 2
来源：https://of.zhonguo5118.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：https://zl.zhonguo3118.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：https://og.zhonguo4118.cn

Java: 7 / 2; 7 % 2
来源：https://kw.zhonguo6118.cn

Go:   7 / 2; 7 % 2
来源：https://vc.zhonguo7118.cn

Ruby: 7 / 2; 7 % 2
来源：https://ft.zhonguo6118.cn

C#:   7 / 2; 7 % 2
来源：https://bi.zhonguo4118.cn

[A06] 字符串转数字
来源：https://db.zhonguo1118.cn

Py:   int("42"); float("3.14")
来源：https://ao.zhonguo2118.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：https://by.zhonguo6118.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：https://lq.zhonguo7118.cn

TS:   parseInt("42", 10); Number("42")
来源：https://dk.zhonguo3118.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：https://km.zhonguo8118.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：https://qg.zhonguo7118.cn

Ruby: "42".to_i; "3.14".to_f
来源：https://jx.zhonguo4118.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：https://hb.zhonguo3118.cn

[A07] 数字转字符串
来源：https://od.zhonguo2118.cn

Py:   str(42)
来源：https://qv.zhonguo3118.cn

PHP:  (string) 42; strval(42)
来源：https://th.zhonguo6118.cn

JS:   String(42); (42).toString()
来源：https://wx.zhonguo3118.cn

TS:   String(42)
来源：https://nj.zhonguo3118.cn

Java: String.valueOf(42); Integer.toString(42)
来源：https://qe.zhonguo8118.cn

Go:   strconv.Itoa(42)
来源：https://me.zhonguo2118.cn

Ruby: 42.to_s
来源：https://xr.zhonguo2118.cn

C#:   42.ToString()
来源：https://vf.zhonguo2118.cn

[A08] 取整与四舍五入
来源：https://pe.zhonguo2118.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：https://az.zhonguo8118.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：https://cz.zhonguo6118.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：https://ch.zhonguo6118.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：https://xg.zhonguo2118.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：https://kd.zhonguo8118.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：https://qo.zhonguo6118.cn

Ruby: 3.567.round(2); 3.9.floor
来源：https://te.zhonguo8118.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：https://cu.zhonguo3118.cn

[A09] 绝对值与最大最小值
来源：https://sg.zhonguo2118.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：https://tq.zhonguo1118.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：https://ae.zhonguo5118.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：https://tx.zhonguo2118.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：https://wy.zhonguo5118.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：https://cg.zhonguo1118.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：https://vv.zhonguo8118.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：https://ja.zhonguo1118.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：https://kf.zhonguo4118.cn

[A10] 生成随机数
来源：https://bc.zhonguo2118.cn

Py:   import random; random.randint(1, 100)
来源：https://yt.zhonguo5118.cn

PHP:  random_int(1, 100);
来源：https://am.zhonguo5118.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：https://jn.zhonguo4118.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：https://xp.zhonguo3118.cn

Java: new Random().nextInt(100) + 1
来源：https://hu.zhonguo6118.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：https://yx.zhonguo7118.cn

Ruby: rand(1..100)
来源：https://ju.zhonguo1118.cn

C#:   new Random().Next(1, 101)
来源：https://gc.zhonguo7118.cn

[A11] 条件表达式（三元）
来源：https://fj.zhonguo4118.cn

Py:   "yes" if x > 0 else "no"
来源：https://cw.zhonguo5118.cn

PHP:  $x > 0 ? "yes" : "no"
来源：https://yz.zhonguo3118.cn

JS:   x > 0 ? "yes" : "no"
来源：https://yf.zhonguo8118.cn

TS:   x > 0 ? "yes" : "no"
来源：https://wy.zhonguo1118.cn

Java: x > 0 ? "yes" : "no"
来源：https://vg.zhonguo1118.cn

Go:   // 无三元运算符，需用 if 语句
来源：https://ki.zhonguo4118.cn

Ruby: x > 0 ? "yes" : "no"
来源：https://xh.zhonguo5118.cn

C#:   x > 0 ? "yes" : "no"
来源：https://va.zhonguo4118.cn

[A12] 字符串插值 / 格式化
来源：https://qa.zhonguo6118.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：https://yn.zhonguo2118.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：https://zj.zhonguo3118.cn

JS:   `Hello, ${name}!`
来源：https://bo.zhonguo6118.cn

TS:   `Hello, ${name}!`
来源：https://sk.zhonguo6118.cn

Java: "Hello, %s!".formatted(name)
来源：https://tc.zhonguo2118.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：https://ej.zhonguo8118.cn

Ruby: "Hello, #{name}!"
来源：https://mh.zhonguo3118.cn

C#:   $"Hello, {name}!"
来源：https://xs.zhonguo2118.cn

[A13] 多行字符串（练习 \n 转义）
来源：https://sl.zhonguo1118.cn

Py:   "第一行\n第二行"
来源：https://mz.zhonguo2118.cn

PHP:  "第一行\n第二行"
来源：https://tj.zhonguo4118.cn

JS:   "第一行\n第二行"
来源：https://de.zhonguo1118.cn

TS:   "第一行\n第二行"
来源：https://uc.zhonguo8118.cn

Java: "第一行\n第二行"
来源：https://wi.zhonguo4118.cn

Go:   "第一行\n第二行"
来源：https://wu.zhonguo2118.cn

Ruby: "第一行\n第二行"
来源：https://ea.zhonguo6118.cn

C#:   "第一行\n第二行"
来源：https://zo.zhonguo7118.cn

[A14] 注释写法
来源：https://xr.zhonguo7118.cn

Py:   # 单行；三引号字符串可作多行说明
来源：https://ol.zhonguo2118.cn

PHP:  // 或 # 单行；/* 多行 */
来源：https://ij.zhonguo5118.cn

JS:   // 单行；/* 多行 */
来源：https://zc.zhonguo6118.cn

TS:   // 单行；/* 多行 */
来源：https://ov.zhonguo4118.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：https://zl.zhonguo1118.cn

Go:   // 单行；/* 多行 */
来源：https://qh.zhonguo5118.cn

Ruby: # 单行；=begin 多行 =end
来源：https://yq.zhonguo3118.cn

C#:   // 单行；/* 多行 */
来源：https://qy.zhonguo7118.cn

[A15] 空值判断与默认值
来源：https://aq.zhonguo7118.cn

Py:   value = data or "默认值"
来源：https://ba.zhonguo2118.cn

PHP:  $value = $data ?? "默认值";
来源：https://of.zhonguo7118.cn

JS:   const value = data ?? "默认值";
来源：https://tt.zhonguo1118.cn

TS:   const value = data ?? "默认值";
来源：https://gg.zhonguo3118.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：https://qu.zhonguo6118.cn

Go:   if data == "" { data = "默认值" }
来源：https://dn.zhonguo7118.cn

Ruby: value = data || "默认值"
来源：https://zj.zhonguo3118.cn

C#:   var value = data ?? "默认值";
来源：https://dp.zhonguo5118.cn

[A16] 真假值判断规则
来源：https://ym.zhonguo6118.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：https://gd.zhonguo1118.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：https://mw.zhonguo7118.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：https://ak.zhonguo3118.cn

TS:   if (!x) {}
来源：https://vz.zhonguo2118.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：https://cy.zhonguo7118.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：https://ue.zhonguo8118.cn

Ruby: unless x            # nil 与 false 为假
来源：https://ok.zhonguo4118.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：https://hl.zhonguo6118.cn

[A17] 位运算
来源：https://qs.zhonguo6118.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://pw.zhonguo6118.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：https://tp.zhonguo4118.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://th.zhonguo7118.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：https://gb.zhonguo3118.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://ap.zhonguo8118.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：https://qi.zhonguo8118.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://nw.zhonguo2118.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://oh.zhonguo5118.cn

[A18] 字符与 ASCII 码互转
来源：https://pi.zhonguo6118.cn

Py:   ord("A"); chr(65)
来源：https://mw.zhonguo8118.cn

PHP:  ord("A"); chr(65)
来源：https://wq.zhonguo1118.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：https://ud.zhonguo2118.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：https://xl.zhonguo3118.cn

Java: (int) 'A'; (char) 65
来源：https://sx.zhonguo4118.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：https://rp.zhonguo8118.cn

Ruby: "A".ord; 65.chr
来源：https://fu.zhonguo2118.cn

C#:   (int)'A'; (char)65
来源：https://je.zhonguo3118.cn

[A19] 交换两个变量
来源：https://cd.zhonguo7118.cn

Py:   a, b = b, a
来源：https://tn.zhonguo4118.cn

PHP:  [$a, $b] = [$b, $a];
来源：https://mk.zhonguo8118.cn

JS:   [a, b] = [b, a];
来源：https://mz.zhonguo3118.cn

TS:   [a, b] = [b, a];
来源：https://vz.zhonguo7118.cn

Java: int t = a; a = b; b = t;
来源：https://nu.zhonguo7118.cn

Go:   a, b = b, a
来源：https://vq.zhonguo8118.cn

Ruby: a, b = b, a
来源：https://sw.zhonguo8118.cn

C#:   (a, b) = (b, a);
来源：https://jx.zhonguo7118.cn

[A20] 读取标准输入
来源：https://rc.zhonguo5118.cn

Py:   name = input("请输入：")
来源：https://dc.zhonguo1118.cn

PHP:  $name = trim(fgets(STDIN));
来源：https://mr.zhonguo3118.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：https://qq.zhonguo8118.cn

TS:   // Node.js：readline 模块
来源：https://vm.zhonguo8118.cn

Java: new Scanner(System.in).nextLine()
来源：https://wb.zhonguo8118.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：https://mb.zhonguo7118.cn

Ruby: gets.chomp
来源：https://dg.zhonguo5118.cn

C#:   Console.ReadLine();
来源：https://ju.zhonguo2118.cn

[A21] 保留指定小数位输出
来源：https://ud.zhonguo8118.cn

Py:   f"{3.14159:.2f}"
来源：https://kh.zhonguo5118.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：https://zf.zhonguo4118.cn

JS:   (3.14159).toFixed(2)
来源：https://nn.zhonguo3118.cn

TS:   (3.14159).toFixed(2)
来源：https://du.zhonguo7118.cn

Java: String.format("%.2f", 3.14159)
来源：https://jn.zhonguo8118.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：https://jd.zhonguo8118.cn

Ruby: format("%.2f", 3.14159)
来源：https://xd.zhonguo5118.cn

C#:   3.14159.ToString("F2")
来源：https://fz.zhonguo6118.cn

[A22] 获取字符串长度
来源：https://fj.zhonguo1118.cn

Py:   len(s)
来源：https://ux.zhonguo7118.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：https://gm.zhonguo7118.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：https://xl.zhonguo2118.cn

TS:   s.length
来源：https://ib.zhonguo6118.cn

Java: s.length()
来源：https://bf.zhonguo6118.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：https://zu.zhonguo5118.cn

Ruby: s.length
来源：https://bs.zhonguo8118.cn

C#:   s.Length
来源：https://ml.zhonguo2118.cn

[A23] 大小写转换
来源：https://by.zhonguo2118.cn

Py:   s.upper(); s.lower(); s.title()
来源：https://uo.zhonguo3118.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：https://gw.zhonguo2118.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：https://aa.zhonguo2118.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：https://gf.zhonguo1118.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：https://oj.zhonguo7118.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：https://rt.zhonguo1118.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：https://se.zhonguo5118.cn

C#:   s.ToUpper(); s.ToLower()
来源：https://sr.zhonguo4118.cn

[A24] 去除首尾空白
来源：https://gp.zhonguo8118.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：https://st.zhonguo8118.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：https://ts.zhonguo1118.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://mv.zhonguo5118.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://cv.zhonguo4118.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：https://pb.zhonguo3118.cn

Go:   strings.TrimSpace(s)
来源：https://ge.zhonguo6118.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：https://bk.zhonguo4118.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：https://qj.zhonguo6118.cn

[A25] 字符串比较
来源：https://le.zhonguo7118.cn

Py:   s1 == s2; s1 != s2
来源：https://tk.zhonguo7118.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：https://tl.zhonguo4118.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：https://ju.zhonguo1118.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：https://sb.zhonguo8118.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：https://xn.zhonguo7118.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：https://xk.zhonguo3118.cn

Ruby: s1 == s2; s1 <=> s2
来源：https://so.zhonguo6118.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：https://fr.zhonguo5118.cn

[A26] 类型转换总览
来源：https://iq.zhonguo4118.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：https://bb.zhonguo2118.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：https://hs.zhonguo8118.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：https://nh.zhonguo6118.cn

TS:   Number() String() Boolean() x as number
来源：https://qf.zhonguo3118.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：https://rg.zhonguo3118.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：https://db.zhonguo3118.cn

Ruby: to_i to_f to_s to_sym to_a
来源：https://if.zhonguo5118.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：https://ho.zhonguo8118.cn

================================================================================
来源：https://hn.zhonguo2118.cn

B. 流程控制
来源：https://pq.zhonguo8118.cn

================================================================================
来源：https://si.zhonguo8118.cn

[B01] 条件判断 if / else
来源：https://uj.zhonguo2118.cn

Py:   result = "正" if x > 0 else "非正"
来源：https://zv.zhonguo1118.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：https://ip.zhonguo8118.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：https://wx.zhonguo7118.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：https://gj.zhonguo3118.cn

Java: String r = x > 0 ? "正" : "非正";
来源：https://dl.zhonguo2118.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：https://je.zhonguo7118.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：https://eh.zhonguo5118.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：https://mn.zhonguo2118.cn

[B02] 多分支 else if / elif
来源：https://dx.zhonguo3118.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：https://gp.zhonguo8118.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：https://ld.zhonguo1118.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://ha.zhonguo1118.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://cp.zhonguo8118.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://jz.zhonguo4118.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：https://yp.zhonguo6118.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：https://nw.zhonguo2118.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://py.zhonguo1118.cn

[B03] switch / match / case
来源：https://fd.zhonguo8118.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：https://fz.zhonguo4118.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：https://te.zhonguo7118.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://dt.zhonguo2118.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://ml.zhonguo8118.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：https://oo.zhonguo2118.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：https://op.zhonguo7118.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：https://mu.zhonguo5118.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：https://ar.zhonguo2118.cn

[B04] for 计数循环
来源：https://xu.zhonguo6118.cn

Py:   for i in range(10): print(i)
来源：https://wh.zhonguo3118.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：https://mi.zhonguo3118.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://wz.zhonguo8118.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://me.zhonguo5118.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：https://tl.zhonguo1118.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：https://uu.zhonguo1118.cn

Ruby: 10.times { |i| puts i }
来源：https://ik.zhonguo4118.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：https://dp.zhonguo3118.cn

[B05] 遍历数组 / 列表
来源：https://ts.zhonguo5118.cn

Py:   for item in arr: print(item)
来源：https://bu.zhonguo4118.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：https://za.zhonguo8118.cn

JS:   for (const item of arr) { console.log(item); }
来源：https://ty.zhonguo3118.cn

TS:   for (const item of arr) { console.log(item); }
来源：https://zn.zhonguo8118.cn

Java: for (var item : arr) { System.out.println(item); }
来源：https://gi.zhonguo8118.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：https://sl.zhonguo7118.cn

Ruby: arr.each { |item| puts item }
来源：https://tj.zhonguo7118.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：https://td.zhonguo6118.cn

[B06] 遍历字典 / 对象
来源：https://jh.zhonguo5118.cn

Py:   for k, v in d.items(): print(k, v)
来源：https://kl.zhonguo8118.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：https://rp.zhonguo2118.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://hj.zhonguo6118.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://yy.zhonguo8118.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：https://vd.zhonguo5118.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：https://hg.zhonguo6118.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：https://wc.zhonguo1118.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：https://ml.zhonguo1118.cn

[B07] while 循环
来源：https://yx.zhonguo2118.cn

Py:   while i < 10: i += 1
来源：https://dw.zhonguo5118.cn

PHP:  while ($i < 10) { $i++; }
来源：https://fw.zhonguo7118.cn

JS:   while (i < 10) { i++; }
来源：https://ln.zhonguo5118.cn

TS:   while (i < 10) { i++; }
来源：https://sm.zhonguo8118.cn

Java: while (i < 10) { i++; }
来源：https://dw.zhonguo7118.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：https://de.zhonguo2118.cn

Ruby: while i < 10; i += 1; end
来源：https://ca.zhonguo2118.cn

C#:   while (i < 10) { i++; }
来源：https://dt.zhonguo4118.cn

[B08] do-while（至少执行一次）
来源：https://tv.zhonguo4118.cn

Py:   # 无 do-while：用 while True + break
来源：https://sw.zhonguo4118.cn

PHP:  do { $i++; } while ($i < 10);
来源：https://zv.zhonguo7118.cn

JS:   do { i++; } while (i < 10);
来源：https://km.zhonguo6118.cn

TS:   do { i++; } while (i < 10);
来源：https://ck.zhonguo3118.cn

Java: do { i++; } while (i < 10);
来源：https://ui.zhonguo1118.cn

Go:   for { i++; if i >= 10 { break } }
来源：https://wc.zhonguo5118.cn

Ruby: begin; i += 1; end while i < 10
来源：https://ln.zhonguo5118.cn

C#:   do { i++; } while (i < 10);
来源：https://qe.zhonguo6118.cn

[B09] break 与 continue
来源：https://qi.zhonguo1118.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：https://sd.zhonguo8118.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：https://ri.zhonguo4118.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://ns.zhonguo2118.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://kh.zhonguo6118.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://ll.zhonguo6118.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：https://ww.zhonguo2118.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：https://av.zhonguo8118.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://jv.zhonguo8118.cn

[B10] 遍历同时拿索引
来源：https://sg.zhonguo6118.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：https://kb.zhonguo3118.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：https://kn.zhonguo6118.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：https://xr.zhonguo6118.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：https://mv.zhonguo8118.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：https://hf.zhonguo5118.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：https://to.zhonguo8118.cn


<!-- 参考信息 -->