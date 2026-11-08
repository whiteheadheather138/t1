代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：https://cg.zhonguo8118.cn

[A03] 常量定义
来源：https://qn.zhonguo1118.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：https://oe.zhonguo2118.cn

PHP:  const PI = 3.14159;
来源：https://ft.zhonguo1118.cn

JS:   const PI = 3.14159;
来源：https://by.zhonguo7118.cn

TS:   const PI: number = 3.14159;
来源：https://oi.zhonguo1118.cn

Java: static final double PI = 3.14159;
来源：https://px.zhonguo3118.cn

Go:   const PI = 3.14159
来源：https://wy.zhonguo6118.cn

Ruby: PI = 3.14159
来源：https://ex.zhonguo6118.cn

C#:   const double PI = 3.14159;
来源：https://sd.zhonguo8118.cn

[A04] 判断变量类型
来源：https://am.zhonguo3118.cn

Py:   type(x).__name__; isinstance(x, int)
来源：https://vm.zhonguo1118.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：https://lu.zhonguo7118.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：https://wz.zhonguo2118.cn

TS:   typeof x; x instanceof Date
来源：https://ai.zhonguo8118.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：https://ya.zhonguo6118.cn

Go:   reflect.TypeOf(x).Name()
来源：https://ch.zhonguo6118.cn

Ruby: x.class; x.is_a?(Integer)
来源：https://qu.zhonguo3118.cn

C#:   x.GetType().Name; x is int
来源：https://jl.zhonguo6118.cn

[A05] 整数除法与取模
来源：https://gs.zhonguo8118.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：https://rr.zhonguo2118.cn

PHP:  intdiv(7, 2); 7 % 2
来源：https://pn.zhonguo2118.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：https://ni.zhonguo1118.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：https://mt.zhonguo6118.cn

Java: 7 / 2; 7 % 2
来源：https://he.zhonguo2118.cn

Go:   7 / 2; 7 % 2
来源：https://nn.zhonguo5118.cn

Ruby: 7 / 2; 7 % 2
来源：https://ov.zhonguo3118.cn

C#:   7 / 2; 7 % 2
来源：https://di.zhonguo2118.cn

[A06] 字符串转数字
来源：https://sj.zhonguo4118.cn

Py:   int("42"); float("3.14")
来源：https://sx.zhonguo6118.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：https://xm.zhonguo7118.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：https://xp.zhonguo8118.cn

TS:   parseInt("42", 10); Number("42")
来源：https://ol.zhonguo6118.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：https://hh.zhonguo3118.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：https://xs.zhonguo1118.cn

Ruby: "42".to_i; "3.14".to_f
来源：https://be.zhonguo8118.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：https://pj.zhonguo4118.cn

[A07] 数字转字符串
来源：https://km.zhonguo6118.cn

Py:   str(42)
来源：https://kt.zhonguo8118.cn

PHP:  (string) 42; strval(42)
来源：https://bt.zhonguo1118.cn

JS:   String(42); (42).toString()
来源：https://sc.zhonguo7118.cn

TS:   String(42)
来源：https://uh.zhonguo1118.cn

Java: String.valueOf(42); Integer.toString(42)
来源：https://pr.zhonguo2118.cn

Go:   strconv.Itoa(42)
来源：https://uy.zhonguo2118.cn

Ruby: 42.to_s
来源：https://kp.zhonguo6118.cn

C#:   42.ToString()
来源：https://fr.zhonguo6118.cn

[A08] 取整与四舍五入
来源：https://js.zhonguo7118.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：https://pb.zhonguo4118.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：https://nq.zhonguo5118.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：https://hg.zhonguo7118.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：https://if.zhonguo4118.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：https://gk.zhonguo5118.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：https://rl.zhonguo3118.cn

Ruby: 3.567.round(2); 3.9.floor
来源：https://ml.zhonguo3118.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：https://rp.zhonguo1118.cn

[A09] 绝对值与最大最小值
来源：https://xl.zhonguo5118.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：https://dq.zhonguo1118.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：https://yo.zhonguo7118.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：https://db.zhonguo6118.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：https://rc.zhonguo7118.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：https://gs.zhonguo5118.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：https://oj.zhonguo1118.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：https://tj.zhonguo7118.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：https://ge.zhonguo6118.cn

[A10] 生成随机数
来源：https://om.zhonguo7118.cn

Py:   import random; random.randint(1, 100)
来源：https://zc.zhonguo1118.cn

PHP:  random_int(1, 100);
来源：https://zm.zhonguo1118.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：https://mb.zhonguo4118.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：https://xq.zhonguo7118.cn

Java: new Random().nextInt(100) + 1
来源：https://gr.zhonguo5118.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：https://nq.zhonguo7118.cn

Ruby: rand(1..100)
来源：https://ue.zhonguo4118.cn

C#:   new Random().Next(1, 101)
来源：https://so.zhonguo3118.cn

[A11] 条件表达式（三元）
来源：https://km.zhonguo8118.cn

Py:   "yes" if x > 0 else "no"
来源：https://es.zhonguo3118.cn

PHP:  $x > 0 ? "yes" : "no"
来源：https://nu.zhonguo8118.cn

JS:   x > 0 ? "yes" : "no"
来源：https://tt.zhonguo5118.cn

TS:   x > 0 ? "yes" : "no"
来源：https://uf.zhonguo7118.cn

Java: x > 0 ? "yes" : "no"
来源：https://pj.zhonguo2118.cn

Go:   // 无三元运算符，需用 if 语句
来源：https://yq.zhonguo5118.cn

Ruby: x > 0 ? "yes" : "no"
来源：https://ow.zhonguo8118.cn

C#:   x > 0 ? "yes" : "no"
来源：https://yf.zhonguo2118.cn

[A12] 字符串插值 / 格式化
来源：https://oc.zhonguo3118.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：https://af.zhonguo8118.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：https://ao.zhonguo8118.cn

JS:   `Hello, ${name}!`
来源：https://di.zhonguo7118.cn

TS:   `Hello, ${name}!`
来源：https://gh.zhonguo6118.cn

Java: "Hello, %s!".formatted(name)
来源：https://nc.zhonguo3118.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：https://ds.zhonguo5118.cn

Ruby: "Hello, #{name}!"
来源：https://so.zhonguo3118.cn

C#:   $"Hello, {name}!"
来源：https://ny.zhonguo1118.cn

[A13] 多行字符串（练习 \n 转义）
来源：https://oo.zhonguo4118.cn

Py:   "第一行\n第二行"
来源：https://il.zhonguo1118.cn

PHP:  "第一行\n第二行"
来源：https://ag.zhonguo8118.cn

JS:   "第一行\n第二行"
来源：https://mv.zhonguo4118.cn

TS:   "第一行\n第二行"
来源：https://tw.zhonguo3118.cn

Java: "第一行\n第二行"
来源：https://dx.zhonguo1118.cn

Go:   "第一行\n第二行"
来源：https://yb.zhonguo2118.cn

Ruby: "第一行\n第二行"
来源：https://ok.zhonguo5118.cn

C#:   "第一行\n第二行"
来源：https://dg.zhonguo2118.cn

[A14] 注释写法
来源：https://up.zhonguo3118.cn

Py:   # 单行；三引号字符串可作多行说明
来源：https://jc.zhonguo6118.cn

PHP:  // 或 # 单行；/* 多行 */
来源：https://fg.zhonguo5118.cn

JS:   // 单行；/* 多行 */
来源：https://nq.zhonguo2118.cn

TS:   // 单行；/* 多行 */
来源：https://fu.zhonguo4118.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：https://iy.zhonguo3118.cn

Go:   // 单行；/* 多行 */
来源：https://pi.zhonguo7118.cn

Ruby: # 单行；=begin 多行 =end
来源：https://td.zhonguo5118.cn

C#:   // 单行；/* 多行 */
来源：https://za.zhonguo5118.cn

[A15] 空值判断与默认值
来源：https://gm.zhonguo6118.cn

Py:   value = data or "默认值"
来源：https://zt.zhonguo4118.cn

PHP:  $value = $data ?? "默认值";
来源：https://ot.zhonguo8118.cn

JS:   const value = data ?? "默认值";
来源：https://gk.zhonguo4118.cn

TS:   const value = data ?? "默认值";
来源：https://vv.zhonguo1118.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：https://xo.zhonguo2118.cn

Go:   if data == "" { data = "默认值" }
来源：https://uc.zhonguo5118.cn

Ruby: value = data || "默认值"
来源：https://dx.zhonguo2118.cn

C#:   var value = data ?? "默认值";
来源：https://ke.zhonguo5118.cn

[A16] 真假值判断规则
来源：https://yd.zhonguo8118.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：https://wj.zhonguo8118.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：https://nf.zhonguo3118.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：https://zl.zhonguo6118.cn

TS:   if (!x) {}
来源：https://rj.zhonguo5118.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：https://ac.zhonguo3118.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：https://xs.zhonguo8118.cn

Ruby: unless x            # nil 与 false 为假
来源：https://tl.zhonguo2118.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：https://io.zhonguo2118.cn

[A17] 位运算
来源：https://qo.zhonguo8118.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://gz.zhonguo7118.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：https://bt.zhonguo7118.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://zf.zhonguo7118.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：https://no.zhonguo3118.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://qi.zhonguo8118.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：https://rk.zhonguo8118.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://jm.zhonguo5118.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://hq.zhonguo7118.cn

[A18] 字符与 ASCII 码互转
来源：https://qc.zhonguo8118.cn

Py:   ord("A"); chr(65)
来源：https://cw.zhonguo8118.cn

PHP:  ord("A"); chr(65)
来源：https://zn.zhonguo6118.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：https://kv.zhonguo7118.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：https://po.zhonguo8118.cn

Java: (int) 'A'; (char) 65
来源：https://pw.zhonguo2118.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：https://oj.zhonguo1118.cn

Ruby: "A".ord; 65.chr
来源：https://ig.zhonguo4118.cn

C#:   (int)'A'; (char)65
来源：https://ls.zhonguo3118.cn

[A19] 交换两个变量
来源：https://iy.zhonguo5118.cn

Py:   a, b = b, a
来源：https://yp.zhonguo7118.cn

PHP:  [$a, $b] = [$b, $a];
来源：https://po.zhonguo5118.cn

JS:   [a, b] = [b, a];
来源：https://vn.zhonguo6118.cn

TS:   [a, b] = [b, a];
来源：https://fv.zhonguo2118.cn

Java: int t = a; a = b; b = t;
来源：https://th.zhonguo1118.cn

Go:   a, b = b, a
来源：https://kn.zhonguo5118.cn

Ruby: a, b = b, a
来源：https://rn.zhonguo7118.cn

C#:   (a, b) = (b, a);
来源：https://oz.zhonguo2118.cn

[A20] 读取标准输入
来源：https://vn.zhonguo1118.cn

Py:   name = input("请输入：")
来源：https://od.zhonguo5118.cn

PHP:  $name = trim(fgets(STDIN));
来源：https://ts.zhonguo5118.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：https://jt.zhonguo6118.cn

TS:   // Node.js：readline 模块
来源：https://vu.zhonguo5118.cn

Java: new Scanner(System.in).nextLine()
来源：https://ue.zhonguo6118.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：https://yy.zhonguo1118.cn

Ruby: gets.chomp
来源：https://aw.zhonguo4118.cn

C#:   Console.ReadLine();
来源：https://ck.zhonguo7118.cn

[A21] 保留指定小数位输出
来源：https://wq.zhonguo8118.cn

Py:   f"{3.14159:.2f}"
来源：https://oc.zhonguo6118.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：https://ty.zhonguo1118.cn

JS:   (3.14159).toFixed(2)
来源：https://rv.zhonguo4118.cn

TS:   (3.14159).toFixed(2)
来源：https://dc.zhonguo5118.cn

Java: String.format("%.2f", 3.14159)
来源：https://my.zhonguo8118.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：https://qb.zhonguo4118.cn

Ruby: format("%.2f", 3.14159)
来源：https://ae.zhonguo7118.cn

C#:   3.14159.ToString("F2")
来源：https://ah.zhonguo5118.cn

[A22] 获取字符串长度
来源：https://wo.zhonguo4118.cn

Py:   len(s)
来源：https://me.zhonguo1118.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：https://qp.zhonguo7118.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：https://fw.zhonguo3118.cn

TS:   s.length
来源：https://di.zhonguo1118.cn

Java: s.length()
来源：https://ic.zhonguo7118.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：https://ee.zhonguo4118.cn

Ruby: s.length
来源：https://ze.zhonguo4118.cn

C#:   s.Length
来源：https://uw.zhonguo5118.cn

[A23] 大小写转换
来源：https://qp.zhonguo8118.cn

Py:   s.upper(); s.lower(); s.title()
来源：https://gd.zhonguo3118.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：https://db.zhonguo3118.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：https://bz.zhonguo4118.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：https://vd.zhonguo3118.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：https://ai.zhonguo8118.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：https://ab.zhonguo7118.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：https://ng.zhonguo6118.cn

C#:   s.ToUpper(); s.ToLower()
来源：https://uj.zhonguo5118.cn

[A24] 去除首尾空白
来源：https://df.zhonguo4118.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：https://yt.zhonguo5118.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：https://qw.zhonguo1118.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://yq.zhonguo3118.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://ck.zhonguo2118.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：https://ss.zhonguo2118.cn

Go:   strings.TrimSpace(s)
来源：https://ym.zhonguo8118.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：https://cb.zhonguo3118.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：https://kh.zhonguo5118.cn

[A25] 字符串比较
来源：https://py.zhonguo7118.cn

Py:   s1 == s2; s1 != s2
来源：https://nm.zhonguo6118.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：https://id.zhonguo6118.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：https://vt.zhonguo3118.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：https://ab.zhonguo6118.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：https://ru.zhonguo4118.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：https://um.zhonguo6118.cn

Ruby: s1 == s2; s1 <=> s2
来源：https://sg.zhonguo2118.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：https://ey.zhonguo3118.cn

[A26] 类型转换总览
来源：https://cg.zhonguo6118.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：https://ko.zhonguo8118.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：https://hh.zhonguo5118.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：https://hx.zhonguo1118.cn

TS:   Number() String() Boolean() x as number
来源：https://id.zhonguo7118.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：https://fv.zhonguo6118.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：https://gz.zhonguo7118.cn

Ruby: to_i to_f to_s to_sym to_a
来源：https://xu.zhonguo5118.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：https://pe.zhonguo4118.cn

================================================================================
来源：https://it.zhonguo2118.cn

B. 流程控制
来源：https://dy.zhonguo6118.cn

================================================================================
来源：https://sh.zhonguo1118.cn

[B01] 条件判断 if / else
来源：https://um.zhonguo8118.cn

Py:   result = "正" if x > 0 else "非正"
来源：https://bt.zhonguo1118.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：https://st.zhonguo6118.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：https://jy.zhonguo1118.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：https://hx.zhonguo2118.cn

Java: String r = x > 0 ? "正" : "非正";
来源：https://al.zhonguo2118.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：https://td.zhonguo5118.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：https://eu.zhonguo6118.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：https://rq.zhonguo3118.cn

[B02] 多分支 else if / elif
来源：https://as.zhonguo4118.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：https://fa.zhonguo2118.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：https://jg.zhonguo7118.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://da.zhonguo1118.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://pr.zhonguo6118.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://wt.zhonguo7118.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：https://sy.zhonguo7118.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：https://yr.zhonguo2118.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://wb.zhonguo1118.cn

[B03] switch / match / case
来源：https://pk.zhonguo7118.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：https://kp.zhonguo8118.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：https://tu.zhonguo8118.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://ha.zhonguo1118.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://qd.zhonguo1118.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：https://on.zhonguo5118.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：https://yn.zhonguo3118.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：https://uw.zhonguo2118.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：https://mp.zhonguo2118.cn

[B04] for 计数循环
来源：https://mo.zhonguo7118.cn

Py:   for i in range(10): print(i)
来源：https://st.zhonguo3118.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：https://gs.zhonguo3118.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://pw.zhonguo3118.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://wq.zhonguo7118.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：https://al.zhonguo3118.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：https://vg.zhonguo2118.cn

Ruby: 10.times { |i| puts i }
来源：https://qe.zhonguo2118.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：https://ke.zhonguo4118.cn

[B05] 遍历数组 / 列表
来源：https://wy.zhonguo4118.cn

Py:   for item in arr: print(item)
来源：https://gx.zhonguo8118.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：https://zs.zhonguo8118.cn

JS:   for (const item of arr) { console.log(item); }
来源：https://ku.zhonguo6118.cn

TS:   for (const item of arr) { console.log(item); }
来源：https://bv.zhonguo5118.cn

Java: for (var item : arr) { System.out.println(item); }
来源：https://zu.zhonguo8118.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：https://ty.zhonguo2118.cn

Ruby: arr.each { |item| puts item }
来源：https://zy.zhonguo4118.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：https://dg.zhonguo2118.cn

[B06] 遍历字典 / 对象
来源：https://kh.zhonguo6118.cn

Py:   for k, v in d.items(): print(k, v)
来源：https://qo.zhonguo5118.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：https://hc.zhonguo7118.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://mj.zhonguo6118.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://jj.zhonguo6118.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：https://yx.zhonguo2118.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：https://to.zhonguo5118.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：https://hl.zhonguo2118.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：https://xs.zhonguo6118.cn

[B07] while 循环
来源：https://oq.zhonguo1118.cn

Py:   while i < 10: i += 1
来源：https://cn.zhonguo2118.cn

PHP:  while ($i < 10) { $i++; }
来源：https://qs.zhonguo2118.cn

JS:   while (i < 10) { i++; }
来源：https://io.zhonguo1118.cn

TS:   while (i < 10) { i++; }
来源：https://mo.zhonguo3118.cn

Java: while (i < 10) { i++; }
来源：https://xt.zhonguo6118.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：https://sc.zhonguo7118.cn

Ruby: while i < 10; i += 1; end
来源：https://up.zhonguo7118.cn

C#:   while (i < 10) { i++; }
来源：https://na.zhonguo4118.cn

[B08] do-while（至少执行一次）
来源：https://as.zhonguo7118.cn

Py:   # 无 do-while：用 while True + break
来源：https://pd.zhonguo6118.cn

PHP:  do { $i++; } while ($i < 10);
来源：https://ki.zhonguo1118.cn

JS:   do { i++; } while (i < 10);
来源：https://ew.zhonguo8118.cn

TS:   do { i++; } while (i < 10);
来源：https://lh.zhonguo1118.cn

Java: do { i++; } while (i < 10);
来源：https://wb.zhonguo7118.cn

Go:   for { i++; if i >= 10 { break } }
来源：https://zd.zhonguo3118.cn

Ruby: begin; i += 1; end while i < 10
来源：https://ar.zhonguo8118.cn

C#:   do { i++; } while (i < 10);
来源：https://lo.zhonguo2118.cn

[B09] break 与 continue
来源：https://qw.zhonguo8118.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：https://sp.zhonguo2118.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：https://eu.zhonguo4118.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://ze.zhonguo8118.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://ey.zhonguo6118.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://wx.zhonguo3118.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：https://yl.zhonguo4118.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：https://gc.zhonguo7118.cn


<!-- 参考信息 -->