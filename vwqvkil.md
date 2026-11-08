代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：https://en.zhonguo1118.cn

[A03] 常量定义
来源：https://nb.zhonguo7118.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：https://wy.zhonguo4118.cn

PHP:  const PI = 3.14159;
来源：https://vk.zhonguo2118.cn

JS:   const PI = 3.14159;
来源：https://do.zhonguo2118.cn

TS:   const PI: number = 3.14159;
来源：https://jc.zhonguo2118.cn

Java: static final double PI = 3.14159;
来源：https://qh.zhonguo6118.cn

Go:   const PI = 3.14159
来源：https://so.zhonguo5118.cn

Ruby: PI = 3.14159
来源：https://pb.zhonguo7118.cn

C#:   const double PI = 3.14159;
来源：https://pn.zhonguo7118.cn

[A04] 判断变量类型
来源：https://nv.zhonguo4118.cn

Py:   type(x).__name__; isinstance(x, int)
来源：https://yd.zhonguo2118.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：https://xe.zhonguo6118.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：https://hc.zhonguo7118.cn

TS:   typeof x; x instanceof Date
来源：https://fu.zhonguo8118.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：https://nk.zhonguo2118.cn

Go:   reflect.TypeOf(x).Name()
来源：https://na.zhonguo1118.cn

Ruby: x.class; x.is_a?(Integer)
来源：https://kh.zhonguo6118.cn

C#:   x.GetType().Name; x is int
来源：https://sa.zhonguo7118.cn

[A05] 整数除法与取模
来源：https://rj.zhonguo1118.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：https://fk.zhonguo5118.cn

PHP:  intdiv(7, 2); 7 % 2
来源：https://ac.zhonguo2118.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：https://ye.zhonguo6118.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：https://pn.zhonguo7118.cn

Java: 7 / 2; 7 % 2
来源：https://yp.zhonguo4118.cn

Go:   7 / 2; 7 % 2
来源：https://lb.zhonguo2118.cn

Ruby: 7 / 2; 7 % 2
来源：https://gv.zhonguo6118.cn

C#:   7 / 2; 7 % 2
来源：https://dk.zhonguo2118.cn

[A06] 字符串转数字
来源：https://dq.zhonguo8118.cn

Py:   int("42"); float("3.14")
来源：https://em.zhonguo5118.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：https://ga.zhonguo1118.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：https://rg.zhonguo7118.cn

TS:   parseInt("42", 10); Number("42")
来源：https://al.zhonguo8118.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：https://wn.zhonguo1118.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：https://oz.zhonguo4118.cn

Ruby: "42".to_i; "3.14".to_f
来源：https://yi.zhonguo5118.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：https://ro.zhonguo7118.cn

[A07] 数字转字符串
来源：https://xe.zhonguo2118.cn

Py:   str(42)
来源：https://ud.zhonguo8118.cn

PHP:  (string) 42; strval(42)
来源：https://sk.zhonguo4118.cn

JS:   String(42); (42).toString()
来源：https://sp.zhonguo6118.cn

TS:   String(42)
来源：https://jy.zhonguo3118.cn

Java: String.valueOf(42); Integer.toString(42)
来源：https://nn.zhonguo6118.cn

Go:   strconv.Itoa(42)
来源：https://ym.zhonguo5118.cn

Ruby: 42.to_s
来源：https://op.zhonguo3118.cn

C#:   42.ToString()
来源：https://uw.zhonguo1118.cn

[A08] 取整与四舍五入
来源：https://xi.zhonguo8118.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：https://ew.zhonguo5118.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：https://ng.zhonguo5118.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：https://kg.zhonguo1118.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：https://ib.zhonguo6118.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：https://tx.zhonguo6118.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：https://xs.zhonguo4118.cn

Ruby: 3.567.round(2); 3.9.floor
来源：https://xb.zhonguo1118.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：https://rv.zhonguo1118.cn

[A09] 绝对值与最大最小值
来源：https://hp.zhonguo6118.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：https://ru.zhonguo7118.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：https://ju.zhonguo1118.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：https://xc.zhonguo6118.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：https://vn.zhonguo7118.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：https://vn.zhonguo5118.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：https://qf.zhonguo1118.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：https://dp.zhonguo7118.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：https://aw.zhonguo7118.cn

[A10] 生成随机数
来源：https://eb.zhonguo2118.cn

Py:   import random; random.randint(1, 100)
来源：https://js.zhonguo6118.cn

PHP:  random_int(1, 100);
来源：https://aw.zhonguo4118.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：https://li.zhonguo8118.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：https://tq.zhonguo1118.cn

Java: new Random().nextInt(100) + 1
来源：https://ea.zhonguo4118.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：https://oh.zhonguo4118.cn

Ruby: rand(1..100)
来源：https://um.zhonguo6118.cn

C#:   new Random().Next(1, 101)
来源：https://oc.zhonguo5118.cn

[A11] 条件表达式（三元）
来源：https://rb.zhonguo2118.cn

Py:   "yes" if x > 0 else "no"
来源：https://rt.zhonguo3118.cn

PHP:  $x > 0 ? "yes" : "no"
来源：https://ve.zhonguo4118.cn

JS:   x > 0 ? "yes" : "no"
来源：https://ql.zhonguo3118.cn

TS:   x > 0 ? "yes" : "no"
来源：https://om.zhonguo6118.cn

Java: x > 0 ? "yes" : "no"
来源：https://bg.zhonguo7118.cn

Go:   // 无三元运算符，需用 if 语句
来源：https://ab.zhonguo4118.cn

Ruby: x > 0 ? "yes" : "no"
来源：https://kg.zhonguo6118.cn

C#:   x > 0 ? "yes" : "no"
来源：https://vw.zhonguo5118.cn

[A12] 字符串插值 / 格式化
来源：https://ie.zhonguo5118.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：https://ep.zhonguo7118.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：https://pd.zhonguo5118.cn

JS:   `Hello, ${name}!`
来源：https://un.zhonguo7118.cn

TS:   `Hello, ${name}!`
来源：https://bu.zhonguo5118.cn

Java: "Hello, %s!".formatted(name)
来源：https://dg.zhonguo6118.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：https://da.zhonguo5118.cn

Ruby: "Hello, #{name}!"
来源：https://qx.zhonguo7118.cn

C#:   $"Hello, {name}!"
来源：https://mi.zhonguo1118.cn

[A13] 多行字符串（练习 \n 转义）
来源：https://zk.zhonguo5118.cn

Py:   "第一行\n第二行"
来源：https://xu.zhonguo8118.cn

PHP:  "第一行\n第二行"
来源：https://we.zhonguo5118.cn

JS:   "第一行\n第二行"
来源：https://kz.zhonguo7118.cn

TS:   "第一行\n第二行"
来源：https://gm.zhonguo7118.cn

Java: "第一行\n第二行"
来源：https://sk.zhonguo2118.cn

Go:   "第一行\n第二行"
来源：https://ay.zhonguo3118.cn

Ruby: "第一行\n第二行"
来源：https://by.zhonguo6118.cn

C#:   "第一行\n第二行"
来源：https://mg.zhonguo6118.cn

[A14] 注释写法
来源：https://ho.zhonguo1118.cn

Py:   # 单行；三引号字符串可作多行说明
来源：https://ni.zhonguo8118.cn

PHP:  // 或 # 单行；/* 多行 */
来源：https://bx.zhonguo2118.cn

JS:   // 单行；/* 多行 */
来源：https://kz.zhonguo8118.cn

TS:   // 单行；/* 多行 */
来源：https://mf.zhonguo1118.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：https://qt.zhonguo2118.cn

Go:   // 单行；/* 多行 */
来源：https://jb.zhonguo8118.cn

Ruby: # 单行；=begin 多行 =end
来源：https://ux.zhonguo4118.cn

C#:   // 单行；/* 多行 */
来源：https://pd.zhonguo7118.cn

[A15] 空值判断与默认值
来源：https://rn.zhonguo5118.cn

Py:   value = data or "默认值"
来源：https://uu.zhonguo8118.cn

PHP:  $value = $data ?? "默认值";
来源：https://uc.zhonguo7118.cn

JS:   const value = data ?? "默认值";
来源：https://vn.zhonguo6118.cn

TS:   const value = data ?? "默认值";
来源：https://zc.zhonguo6118.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：https://iw.zhonguo5118.cn

Go:   if data == "" { data = "默认值" }
来源：https://uw.zhonguo7118.cn

Ruby: value = data || "默认值"
来源：https://gn.zhonguo1118.cn

C#:   var value = data ?? "默认值";
来源：https://ow.zhonguo3118.cn

[A16] 真假值判断规则
来源：https://fz.zhonguo5118.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：https://by.zhonguo5118.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：https://uo.zhonguo2118.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：https://sc.zhonguo1118.cn

TS:   if (!x) {}
来源：https://cj.zhonguo4118.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：https://zn.zhonguo6118.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：https://la.zhonguo5118.cn

Ruby: unless x            # nil 与 false 为假
来源：https://cp.zhonguo7118.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：https://cm.zhonguo2118.cn

[A17] 位运算
来源：https://dt.zhonguo3118.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://jn.zhonguo4118.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：https://ak.zhonguo2118.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://yq.zhonguo6118.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：https://om.zhonguo4118.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://kv.zhonguo4118.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：https://ne.zhonguo7118.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://kv.zhonguo3118.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://cd.zhonguo4118.cn

[A18] 字符与 ASCII 码互转
来源：https://nb.zhonguo4118.cn

Py:   ord("A"); chr(65)
来源：https://de.zhonguo2118.cn

PHP:  ord("A"); chr(65)
来源：https://at.zhonguo6118.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：https://rz.zhonguo7118.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：https://aw.zhonguo1118.cn

Java: (int) 'A'; (char) 65
来源：https://ai.zhonguo8118.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：https://xu.zhonguo3118.cn

Ruby: "A".ord; 65.chr
来源：https://jr.zhonguo2118.cn

C#:   (int)'A'; (char)65
来源：https://mz.zhonguo4118.cn

[A19] 交换两个变量
来源：https://ws.zhonguo2118.cn

Py:   a, b = b, a
来源：https://ks.zhonguo8118.cn

PHP:  [$a, $b] = [$b, $a];
来源：https://eg.zhonguo8118.cn

JS:   [a, b] = [b, a];
来源：https://ls.zhonguo4118.cn

TS:   [a, b] = [b, a];
来源：https://au.zhonguo4118.cn

Java: int t = a; a = b; b = t;
来源：https://nb.zhonguo5118.cn

Go:   a, b = b, a
来源：https://xa.zhonguo2118.cn

Ruby: a, b = b, a
来源：https://te.zhonguo4118.cn

C#:   (a, b) = (b, a);
来源：https://ys.zhonguo3118.cn

[A20] 读取标准输入
来源：https://aq.zhonguo3118.cn

Py:   name = input("请输入：")
来源：https://cg.zhonguo1118.cn

PHP:  $name = trim(fgets(STDIN));
来源：https://ih.zhonguo2118.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：https://if.zhonguo6118.cn

TS:   // Node.js：readline 模块
来源：https://jp.zhonguo4118.cn

Java: new Scanner(System.in).nextLine()
来源：https://ud.zhonguo4118.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：https://ij.zhonguo6118.cn

Ruby: gets.chomp
来源：https://et.zhonguo3118.cn

C#:   Console.ReadLine();
来源：https://aw.zhonguo2118.cn

[A21] 保留指定小数位输出
来源：https://vx.zhonguo6118.cn

Py:   f"{3.14159:.2f}"
来源：https://xe.zhonguo1118.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：https://nb.zhonguo1118.cn

JS:   (3.14159).toFixed(2)
来源：https://pa.zhonguo2118.cn

TS:   (3.14159).toFixed(2)
来源：https://os.zhonguo1118.cn

Java: String.format("%.2f", 3.14159)
来源：https://ln.zhonguo1118.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：https://ok.zhonguo2118.cn

Ruby: format("%.2f", 3.14159)
来源：https://oz.zhonguo7118.cn

C#:   3.14159.ToString("F2")
来源：https://kk.zhonguo2118.cn

[A22] 获取字符串长度
来源：https://ng.zhonguo5118.cn

Py:   len(s)
来源：https://ch.zhonguo7118.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：https://hx.zhonguo3118.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：https://se.zhonguo1118.cn

TS:   s.length
来源：https://sk.zhonguo5118.cn

Java: s.length()
来源：https://sh.zhonguo8118.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：https://qx.zhonguo4118.cn

Ruby: s.length
来源：https://jb.zhonguo5118.cn

C#:   s.Length
来源：https://ej.zhonguo5118.cn

[A23] 大小写转换
来源：https://ct.zhonguo5118.cn

Py:   s.upper(); s.lower(); s.title()
来源：https://kn.zhonguo8118.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：https://cd.zhonguo6118.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：https://xz.zhonguo3118.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：https://ab.zhonguo5118.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：https://ss.zhonguo4118.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：https://qg.zhonguo7118.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：https://co.zhonguo8118.cn

C#:   s.ToUpper(); s.ToLower()
来源：https://rw.zhonguo4118.cn

[A24] 去除首尾空白
来源：https://zu.zhonguo7118.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：https://nh.zhonguo5118.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：https://ol.zhonguo4118.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://ac.zhonguo6118.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://nf.zhonguo1118.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：https://qz.zhonguo1118.cn

Go:   strings.TrimSpace(s)
来源：https://qw.zhonguo7118.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：https://gh.zhonguo5118.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：https://ou.zhonguo1118.cn

[A25] 字符串比较
来源：https://ry.zhonguo2118.cn

Py:   s1 == s2; s1 != s2
来源：https://ov.zhonguo1118.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：https://wl.zhonguo6118.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：https://yy.zhonguo5118.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：https://ld.zhonguo1118.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：https://km.zhonguo1118.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：https://ku.zhonguo7118.cn

Ruby: s1 == s2; s1 <=> s2
来源：https://tu.zhonguo4118.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：https://us.zhonguo7118.cn

[A26] 类型转换总览
来源：https://dh.zhonguo5118.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：https://dr.zhonguo2118.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：https://hq.zhonguo5118.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：https://yg.zhonguo8118.cn

TS:   Number() String() Boolean() x as number
来源：https://bs.zhonguo1118.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：https://xx.zhonguo4118.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：https://bj.zhonguo3118.cn

Ruby: to_i to_f to_s to_sym to_a
来源：https://mo.zhonguo6118.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：https://yi.zhonguo4118.cn

================================================================================
来源：https://rh.zhonguo7118.cn

B. 流程控制
来源：https://es.zhonguo8118.cn

================================================================================
来源：https://kb.zhonguo6118.cn

[B01] 条件判断 if / else
来源：https://dv.zhonguo6118.cn

Py:   result = "正" if x > 0 else "非正"
来源：https://nv.zhonguo5118.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：https://jf.zhonguo2118.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：https://ku.zhonguo2118.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：https://an.zhonguo8118.cn

Java: String r = x > 0 ? "正" : "非正";
来源：https://ah.zhonguo1118.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：https://su.zhonguo3118.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：https://zc.zhonguo8118.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：https://wf.zhonguo7118.cn

[B02] 多分支 else if / elif
来源：https://hr.zhonguo4118.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：https://zd.zhonguo8118.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：https://su.zhonguo3118.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://tv.zhonguo4118.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://by.zhonguo5118.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://hr.zhonguo6118.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：https://ot.zhonguo2118.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：https://lo.zhonguo1118.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://uz.zhonguo5118.cn

[B03] switch / match / case
来源：https://va.zhonguo8118.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：https://pp.zhonguo8118.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：https://ns.zhonguo7118.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://oi.zhonguo2118.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://ro.zhonguo8118.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：https://qn.zhonguo3118.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：https://id.zhonguo1118.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：https://mp.zhonguo7118.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：https://dh.zhonguo7118.cn

[B04] for 计数循环
来源：https://xx.zhonguo5118.cn

Py:   for i in range(10): print(i)
来源：https://zc.zhonguo1118.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：https://ad.zhonguo1118.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://vw.zhonguo8118.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://xs.zhonguo6118.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：https://pb.zhonguo7118.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：https://hx.zhonguo1118.cn

Ruby: 10.times { |i| puts i }
来源：https://ic.zhonguo5118.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：https://od.zhonguo2118.cn

[B05] 遍历数组 / 列表
来源：https://ik.zhonguo8118.cn

Py:   for item in arr: print(item)
来源：https://xz.zhonguo4118.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：https://dx.zhonguo1118.cn

JS:   for (const item of arr) { console.log(item); }
来源：https://rq.zhonguo7118.cn

TS:   for (const item of arr) { console.log(item); }
来源：https://zw.zhonguo1118.cn

Java: for (var item : arr) { System.out.println(item); }
来源：https://iq.zhonguo1118.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：https://dr.zhonguo2118.cn

Ruby: arr.each { |item| puts item }
来源：https://bw.zhonguo3118.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：https://mp.zhonguo1118.cn

[B06] 遍历字典 / 对象
来源：https://uv.zhonguo2118.cn

Py:   for k, v in d.items(): print(k, v)
来源：https://vl.zhonguo7118.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：https://bb.zhonguo5118.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://mt.zhonguo7118.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://iv.zhonguo6118.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：https://fc.zhonguo6118.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：https://as.zhonguo8118.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：https://bs.zhonguo6118.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：https://do.zhonguo6118.cn

[B07] while 循环
来源：https://pq.zhonguo5118.cn

Py:   while i < 10: i += 1
来源：https://uc.zhonguo7118.cn

PHP:  while ($i < 10) { $i++; }
来源：https://pw.zhonguo6118.cn

JS:   while (i < 10) { i++; }
来源：https://hy.zhonguo8118.cn

TS:   while (i < 10) { i++; }
来源：https://of.zhonguo5118.cn

Java: while (i < 10) { i++; }
来源：https://gm.zhonguo2118.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：https://eb.zhonguo5118.cn

Ruby: while i < 10; i += 1; end
来源：https://ke.zhonguo6118.cn

C#:   while (i < 10) { i++; }
来源：https://ka.zhonguo7118.cn

[B08] do-while（至少执行一次）
来源：https://hz.zhonguo8118.cn

Py:   # 无 do-while：用 while True + break
来源：https://zt.zhonguo4118.cn

PHP:  do { $i++; } while ($i < 10);
来源：https://xe.zhonguo7118.cn

JS:   do { i++; } while (i < 10);
来源：https://iu.zhonguo1118.cn

TS:   do { i++; } while (i < 10);
来源：https://ea.zhonguo1118.cn

Java: do { i++; } while (i < 10);
来源：https://kd.zhonguo3118.cn

Go:   for { i++; if i >= 10 { break } }
来源：https://lf.zhonguo3118.cn

Ruby: begin; i += 1; end while i < 10
来源：https://ng.zhonguo7118.cn

C#:   do { i++; } while (i < 10);
来源：https://pw.zhonguo4118.cn

[B09] break 与 continue
来源：https://fj.zhonguo1118.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：https://zv.zhonguo3118.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：https://mr.zhonguo3118.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://hj.zhonguo1118.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://aw.zhonguo3118.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://fk.zhonguo8118.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：https://hj.zhonguo2118.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：https://kx.zhonguo1118.cn


<!-- 参考信息 -->