代发 wailian999

TS:   let name: string = "Alex"; const age: number = 20;
来源：https://mr.zhonguo7118.cn

Java: String name = "Alex"; int age = 20;
来源：https://xk.zhonguo5118.cn

Go:   name := "Alex"; age := 20
来源：https://vq.zhonguo8118.cn

Ruby: name = "Alex"; age = 20
来源：https://ei.zhonguo4118.cn

C#:   string name = "Alex"; int age = 20;
来源：https://ra.zhonguo2118.cn

[A03] 常量定义
来源：https://gf.zhonguo6118.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：https://uj.zhonguo7118.cn

PHP:  const PI = 3.14159;
来源：https://jy.zhonguo8118.cn

JS:   const PI = 3.14159;
来源：https://yi.zhonguo4118.cn

TS:   const PI: number = 3.14159;
来源：https://em.zhonguo7118.cn

Java: static final double PI = 3.14159;
来源：https://oi.zhonguo2118.cn

Go:   const PI = 3.14159
来源：https://de.zhonguo1118.cn

Ruby: PI = 3.14159
来源：https://lz.zhonguo6118.cn

C#:   const double PI = 3.14159;
来源：https://tr.zhonguo7118.cn

[A04] 判断变量类型
来源：https://ht.zhonguo1118.cn

Py:   type(x).__name__; isinstance(x, int)
来源：https://lw.zhonguo1118.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：https://nh.zhonguo6118.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：https://ga.zhonguo6118.cn

TS:   typeof x; x instanceof Date
来源：https://pl.zhonguo5118.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：https://yc.zhonguo6118.cn

Go:   reflect.TypeOf(x).Name()
来源：https://gk.zhonguo8118.cn

Ruby: x.class; x.is_a?(Integer)
来源：https://by.zhonguo7118.cn

C#:   x.GetType().Name; x is int
来源：https://dp.zhonguo6118.cn

[A05] 整数除法与取模
来源：https://qf.zhonguo5118.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：https://ys.zhonguo3118.cn

PHP:  intdiv(7, 2); 7 % 2
来源：https://to.zhonguo5118.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：https://fx.zhonguo5118.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：https://ne.zhonguo4118.cn

Java: 7 / 2; 7 % 2
来源：https://pk.zhonguo7118.cn

Go:   7 / 2; 7 % 2
来源：https://ih.zhonguo8118.cn

Ruby: 7 / 2; 7 % 2
来源：https://xm.zhonguo7118.cn

C#:   7 / 2; 7 % 2
来源：https://sp.zhonguo8118.cn

[A06] 字符串转数字
来源：https://db.zhonguo8118.cn

Py:   int("42"); float("3.14")
来源：https://zq.zhonguo6118.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：https://xa.zhonguo6118.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：https://kh.zhonguo5118.cn

TS:   parseInt("42", 10); Number("42")
来源：https://dl.zhonguo3118.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：https://gj.zhonguo6118.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：https://dp.zhonguo8118.cn

Ruby: "42".to_i; "3.14".to_f
来源：https://sy.zhonguo2118.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：https://rh.zhonguo4118.cn

[A07] 数字转字符串
来源：https://wv.zhonguo8118.cn

Py:   str(42)
来源：https://cz.zhonguo3118.cn

PHP:  (string) 42; strval(42)
来源：https://wd.zhonguo8118.cn

JS:   String(42); (42).toString()
来源：https://qo.zhonguo2118.cn

TS:   String(42)
来源：https://zi.zhonguo8118.cn

Java: String.valueOf(42); Integer.toString(42)
来源：https://rz.zhonguo8118.cn

Go:   strconv.Itoa(42)
来源：https://yo.zhonguo7118.cn

Ruby: 42.to_s
来源：https://nq.zhonguo4118.cn

C#:   42.ToString()
来源：https://xi.zhonguo5118.cn

[A08] 取整与四舍五入
来源：https://cx.zhonguo1118.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：https://ss.zhonguo3118.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：https://by.zhonguo1118.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：https://wf.zhonguo4118.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：https://pb.zhonguo2118.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：https://oi.zhonguo5118.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：https://kq.zhonguo5118.cn

Ruby: 3.567.round(2); 3.9.floor
来源：https://vd.zhonguo6118.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：https://de.zhonguo2118.cn

[A09] 绝对值与最大最小值
来源：https://eu.zhonguo1118.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：https://rz.zhonguo5118.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：https://ji.zhonguo1118.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：https://en.zhonguo5118.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：https://op.zhonguo2118.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：https://mh.zhonguo8118.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：https://gt.zhonguo2118.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：https://cb.zhonguo3118.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：https://yd.zhonguo1118.cn

[A10] 生成随机数
来源：https://nr.zhonguo6118.cn

Py:   import random; random.randint(1, 100)
来源：https://jp.zhonguo3118.cn

PHP:  random_int(1, 100);
来源：https://mj.zhonguo5118.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：https://hd.zhonguo1118.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：https://kb.zhonguo7118.cn

Java: new Random().nextInt(100) + 1
来源：https://dx.zhonguo4118.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：https://ku.zhonguo7118.cn

Ruby: rand(1..100)
来源：https://mk.zhonguo3118.cn

C#:   new Random().Next(1, 101)
来源：https://xt.zhonguo5118.cn

[A11] 条件表达式（三元）
来源：https://ww.zhonguo1118.cn

Py:   "yes" if x > 0 else "no"
来源：https://ij.zhonguo2118.cn

PHP:  $x > 0 ? "yes" : "no"
来源：https://om.zhonguo3118.cn

JS:   x > 0 ? "yes" : "no"
来源：https://nm.zhonguo5118.cn

TS:   x > 0 ? "yes" : "no"
来源：https://ww.zhonguo6118.cn

Java: x > 0 ? "yes" : "no"
来源：https://nw.zhonguo7118.cn

Go:   // 无三元运算符，需用 if 语句
来源：https://rd.zhonguo1118.cn

Ruby: x > 0 ? "yes" : "no"
来源：https://du.zhonguo4118.cn

C#:   x > 0 ? "yes" : "no"
来源：https://iy.zhonguo8118.cn

[A12] 字符串插值 / 格式化
来源：https://jh.zhonguo1118.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：https://cq.zhonguo8118.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：https://mc.zhonguo4118.cn

JS:   `Hello, ${name}!`
来源：https://jw.zhonguo2118.cn

TS:   `Hello, ${name}!`
来源：https://vs.zhonguo3118.cn

Java: "Hello, %s!".formatted(name)
来源：https://wq.zhonguo8118.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：https://ue.zhonguo4118.cn

Ruby: "Hello, #{name}!"
来源：https://nd.zhonguo1118.cn

C#:   $"Hello, {name}!"
来源：https://fb.zhonguo4118.cn

[A13] 多行字符串（练习 \n 转义）
来源：https://se.zhonguo2118.cn

Py:   "第一行\n第二行"
来源：https://mr.zhonguo1118.cn

PHP:  "第一行\n第二行"
来源：https://dx.zhonguo2118.cn

JS:   "第一行\n第二行"
来源：https://ym.zhonguo1118.cn

TS:   "第一行\n第二行"
来源：https://xh.zhonguo8118.cn

Java: "第一行\n第二行"
来源：https://rm.zhonguo1118.cn

Go:   "第一行\n第二行"
来源：https://gl.zhonguo4118.cn

Ruby: "第一行\n第二行"
来源：https://io.zhonguo4118.cn

C#:   "第一行\n第二行"
来源：https://ni.zhonguo4118.cn

[A14] 注释写法
来源：https://bc.zhonguo2118.cn

Py:   # 单行；三引号字符串可作多行说明
来源：https://db.zhonguo7118.cn

PHP:  // 或 # 单行；/* 多行 */
来源：https://vb.zhonguo2118.cn

JS:   // 单行；/* 多行 */
来源：https://nx.zhonguo5118.cn

TS:   // 单行；/* 多行 */
来源：https://dt.zhonguo5118.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：https://nk.zhonguo6118.cn

Go:   // 单行；/* 多行 */
来源：https://ro.zhonguo4118.cn

Ruby: # 单行；=begin 多行 =end
来源：https://gk.zhonguo2118.cn

C#:   // 单行；/* 多行 */
来源：https://fn.zhonguo6118.cn

[A15] 空值判断与默认值
来源：https://ln.zhonguo8118.cn

Py:   value = data or "默认值"
来源：https://eb.zhonguo1118.cn

PHP:  $value = $data ?? "默认值";
来源：https://al.zhonguo2118.cn

JS:   const value = data ?? "默认值";
来源：https://xx.zhonguo7118.cn

TS:   const value = data ?? "默认值";
来源：https://lk.zhonguo6118.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：https://dx.zhonguo6118.cn

Go:   if data == "" { data = "默认值" }
来源：https://fk.zhonguo6118.cn

Ruby: value = data || "默认值"
来源：https://by.zhonguo6118.cn

C#:   var value = data ?? "默认值";
来源：https://gp.zhonguo5118.cn

[A16] 真假值判断规则
来源：https://xg.zhonguo6118.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：https://vk.zhonguo2118.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：https://fm.zhonguo7118.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：https://wd.zhonguo7118.cn

TS:   if (!x) {}
来源：https://bn.zhonguo1118.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：https://db.zhonguo5118.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：https://mg.zhonguo4118.cn

Ruby: unless x            # nil 与 false 为假
来源：https://lm.zhonguo3118.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：https://lx.zhonguo2118.cn

[A17] 位运算
来源：https://cd.zhonguo6118.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://ja.zhonguo3118.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：https://ou.zhonguo1118.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://sk.zhonguo3118.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：https://at.zhonguo1118.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://wj.zhonguo8118.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：https://qc.zhonguo6118.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://tw.zhonguo1118.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://ie.zhonguo6118.cn

[A18] 字符与 ASCII 码互转
来源：https://yh.zhonguo5118.cn

Py:   ord("A"); chr(65)
来源：https://pt.zhonguo5118.cn

PHP:  ord("A"); chr(65)
来源：https://gd.zhonguo1118.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：https://mt.zhonguo8118.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：https://jh.zhonguo7118.cn

Java: (int) 'A'; (char) 65
来源：https://jc.zhonguo7118.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：https://ld.zhonguo6118.cn

Ruby: "A".ord; 65.chr
来源：https://si.zhonguo2118.cn

C#:   (int)'A'; (char)65
来源：https://qv.zhonguo2118.cn

[A19] 交换两个变量
来源：https://es.zhonguo8118.cn

Py:   a, b = b, a
来源：https://gr.zhonguo1118.cn

PHP:  [$a, $b] = [$b, $a];
来源：https://oy.zhonguo3118.cn

JS:   [a, b] = [b, a];
来源：https://lk.zhonguo1118.cn

TS:   [a, b] = [b, a];
来源：https://tb.zhonguo3118.cn

Java: int t = a; a = b; b = t;
来源：https://ds.zhonguo5118.cn

Go:   a, b = b, a
来源：https://jy.zhonguo3118.cn

Ruby: a, b = b, a
来源：https://iw.zhonguo5118.cn

C#:   (a, b) = (b, a);
来源：https://lw.zhonguo2118.cn

[A20] 读取标准输入
来源：https://xt.zhonguo5118.cn

Py:   name = input("请输入：")
来源：https://zj.zhonguo1118.cn

PHP:  $name = trim(fgets(STDIN));
来源：https://mi.zhonguo2118.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：https://qg.zhonguo8118.cn

TS:   // Node.js：readline 模块
来源：https://gn.zhonguo4118.cn

Java: new Scanner(System.in).nextLine()
来源：https://qj.zhonguo5118.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：https://kg.zhonguo2118.cn

Ruby: gets.chomp
来源：https://ot.zhonguo4118.cn

C#:   Console.ReadLine();
来源：https://qv.zhonguo7118.cn

[A21] 保留指定小数位输出
来源：https://kq.zhonguo4118.cn

Py:   f"{3.14159:.2f}"
来源：https://sa.zhonguo4118.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：https://zw.zhonguo7118.cn

JS:   (3.14159).toFixed(2)
来源：https://uu.zhonguo7118.cn

TS:   (3.14159).toFixed(2)
来源：https://hi.zhonguo5118.cn

Java: String.format("%.2f", 3.14159)
来源：https://zh.zhonguo1118.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：https://mg.zhonguo8118.cn

Ruby: format("%.2f", 3.14159)
来源：https://tk.zhonguo1118.cn

C#:   3.14159.ToString("F2")
来源：https://ul.zhonguo1118.cn

[A22] 获取字符串长度
来源：https://jg.zhonguo3118.cn

Py:   len(s)
来源：https://nm.zhonguo4118.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：https://ci.zhonguo3118.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：https://at.zhonguo3118.cn

TS:   s.length
来源：https://hk.zhonguo4118.cn

Java: s.length()
来源：https://qa.zhonguo4118.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：https://se.zhonguo7118.cn

Ruby: s.length
来源：https://ib.zhonguo8118.cn

C#:   s.Length
来源：https://yg.zhonguo2118.cn

[A23] 大小写转换
来源：https://eq.zhonguo4118.cn

Py:   s.upper(); s.lower(); s.title()
来源：https://kk.zhonguo8118.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：https://no.zhonguo5118.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：https://sz.zhonguo8118.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：https://zf.zhonguo3118.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：https://ic.zhonguo6118.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：https://it.zhonguo6118.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：https://wx.zhonguo8118.cn

C#:   s.ToUpper(); s.ToLower()
来源：https://tr.zhonguo3118.cn

[A24] 去除首尾空白
来源：https://ym.zhonguo5118.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：https://nc.zhonguo3118.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：https://zq.zhonguo6118.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://fu.zhonguo7118.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://ym.zhonguo1118.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：https://he.zhonguo1118.cn

Go:   strings.TrimSpace(s)
来源：https://qn.zhonguo3118.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：https://kl.zhonguo1118.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：https://hi.zhonguo2118.cn

[A25] 字符串比较
来源：https://bc.zhonguo2118.cn

Py:   s1 == s2; s1 != s2
来源：https://ly.zhonguo5118.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：https://uq.zhonguo3118.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：https://ai.zhonguo6118.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：https://ig.zhonguo3118.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：https://zy.zhonguo6118.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：https://qu.zhonguo2118.cn

Ruby: s1 == s2; s1 <=> s2
来源：https://sd.zhonguo3118.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：https://tg.zhonguo3118.cn

[A26] 类型转换总览
来源：https://di.zhonguo2118.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：https://lo.zhonguo7118.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：https://tj.zhonguo2118.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：https://og.zhonguo7118.cn

TS:   Number() String() Boolean() x as number
来源：https://ev.zhonguo4118.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：https://rh.zhonguo2118.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：https://ko.zhonguo5118.cn

Ruby: to_i to_f to_s to_sym to_a
来源：https://un.zhonguo8118.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：https://hz.zhonguo3118.cn

================================================================================
来源：https://yg.zhonguo8118.cn

B. 流程控制
来源：https://nk.zhonguo2118.cn

================================================================================
来源：https://zz.zhonguo7118.cn

[B01] 条件判断 if / else
来源：https://gj.zhonguo5118.cn

Py:   result = "正" if x > 0 else "非正"
来源：https://vc.zhonguo3118.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：https://yn.zhonguo7118.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：https://ey.zhonguo2118.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：https://jw.zhonguo2118.cn

Java: String r = x > 0 ? "正" : "非正";
来源：https://hz.zhonguo4118.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：https://pl.zhonguo1118.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：https://nt.zhonguo3118.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：https://kh.zhonguo2118.cn

[B02] 多分支 else if / elif
来源：https://wv.zhonguo2118.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：https://qw.zhonguo5118.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：https://ck.zhonguo3118.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://qi.zhonguo6118.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://mg.zhonguo6118.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://mv.zhonguo7118.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：https://zg.zhonguo8118.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：https://ia.zhonguo6118.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://og.zhonguo5118.cn

[B03] switch / match / case
来源：https://zm.zhonguo3118.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：https://vx.zhonguo5118.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：https://mo.zhonguo1118.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://mk.zhonguo1118.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://mc.zhonguo3118.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：https://pd.zhonguo5118.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：https://yv.zhonguo8118.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：https://af.zhonguo4118.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：https://cp.zhonguo1118.cn

[B04] for 计数循环
来源：https://bn.zhonguo4118.cn

Py:   for i in range(10): print(i)
来源：https://gb.zhonguo5118.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：https://ww.zhonguo8118.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://fj.zhonguo4118.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://dr.zhonguo5118.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：https://ju.zhonguo3118.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：https://it.zhonguo4118.cn

Ruby: 10.times { |i| puts i }
来源：https://mx.zhonguo7118.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：https://ku.zhonguo6118.cn

[B05] 遍历数组 / 列表
来源：https://yp.zhonguo6118.cn

Py:   for item in arr: print(item)
来源：https://jl.zhonguo6118.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：https://bl.zhonguo2118.cn

JS:   for (const item of arr) { console.log(item); }
来源：https://pj.zhonguo5118.cn

TS:   for (const item of arr) { console.log(item); }
来源：https://bn.zhonguo5118.cn

Java: for (var item : arr) { System.out.println(item); }
来源：https://ea.zhonguo7118.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：https://vv.zhonguo5118.cn

Ruby: arr.each { |item| puts item }
来源：https://ge.zhonguo4118.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：https://gk.zhonguo3118.cn

[B06] 遍历字典 / 对象
来源：https://av.zhonguo1118.cn

Py:   for k, v in d.items(): print(k, v)
来源：https://gi.zhonguo2118.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：https://uv.zhonguo7118.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://us.zhonguo8118.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://hw.zhonguo3118.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：https://we.zhonguo6118.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：https://am.zhonguo6118.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：https://jt.zhonguo6118.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：https://ip.zhonguo2118.cn

[B07] while 循环
来源：https://ej.zhonguo4118.cn

Py:   while i < 10: i += 1
来源：https://fk.zhonguo5118.cn

PHP:  while ($i < 10) { $i++; }
来源：https://sk.zhonguo8118.cn

JS:   while (i < 10) { i++; }
来源：https://yc.zhonguo5118.cn

TS:   while (i < 10) { i++; }
来源：https://fd.zhonguo7118.cn

Java: while (i < 10) { i++; }
来源：https://xp.zhonguo7118.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：https://bn.zhonguo2118.cn

Ruby: while i < 10; i += 1; end
来源：https://pp.zhonguo2118.cn

C#:   while (i < 10) { i++; }
来源：https://na.zhonguo5118.cn

[B08] do-while（至少执行一次）
来源：https://lq.zhonguo3118.cn

Py:   # 无 do-while：用 while True + break
来源：https://ng.zhonguo2118.cn

PHP:  do { $i++; } while ($i < 10);
来源：https://nu.zhonguo8118.cn

JS:   do { i++; } while (i < 10);
来源：https://jc.zhonguo2118.cn

TS:   do { i++; } while (i < 10);
来源：https://gt.zhonguo2118.cn

Java: do { i++; } while (i < 10);
来源：https://nu.zhonguo2118.cn

Go:   for { i++; if i >= 10 { break } }
来源：https://ht.zhonguo2118.cn

Ruby: begin; i += 1; end while i < 10
来源：https://ml.zhonguo2118.cn

C#:   do { i++; } while (i < 10);
来源：https://yq.zhonguo2118.cn

[B09] break 与 continue
来源：https://tb.zhonguo5118.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：https://be.zhonguo6118.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：https://fe.zhonguo4118.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://me.zhonguo7118.cn


<!-- 参考信息 -->