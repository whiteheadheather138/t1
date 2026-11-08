代发 wailian999

[A02] 变量声明与赋值
来源：https://mg.zhonguo4118.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：https://yk.zhonguo3118.cn

PHP:  $name = "Alex"; $age = 20;
来源：https://ck.zhonguo3118.cn

JS:   let name = "Alex"; const age = 20;
来源：https://de.zhonguo6118.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：https://gq.zhonguo7118.cn

Java: String name = "Alex"; int age = 20;
来源：https://ww.zhonguo3118.cn

Go:   name := "Alex"; age := 20
来源：https://tu.zhonguo2118.cn

Ruby: name = "Alex"; age = 20
来源：https://es.zhonguo6118.cn

C#:   string name = "Alex"; int age = 20;
来源：https://tf.zhonguo2118.cn

[A03] 常量定义
来源：https://ru.zhonguo6118.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：https://cl.zhonguo6118.cn

PHP:  const PI = 3.14159;
来源：https://zm.zhonguo8118.cn

JS:   const PI = 3.14159;
来源：https://lg.zhonguo2118.cn

TS:   const PI: number = 3.14159;
来源：https://fn.zhonguo2118.cn

Java: static final double PI = 3.14159;
来源：https://au.zhonguo4118.cn

Go:   const PI = 3.14159
来源：https://te.zhonguo7118.cn

Ruby: PI = 3.14159
来源：https://li.zhonguo5118.cn

C#:   const double PI = 3.14159;
来源：https://yo.zhonguo1118.cn

[A04] 判断变量类型
来源：https://ul.zhonguo5118.cn

Py:   type(x).__name__; isinstance(x, int)
来源：https://ot.zhonguo2118.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：https://ms.zhonguo8118.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：https://ws.zhonguo6118.cn

TS:   typeof x; x instanceof Date
来源：https://pz.zhonguo3118.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：https://jq.zhonguo5118.cn

Go:   reflect.TypeOf(x).Name()
来源：https://fl.zhonguo3118.cn

Ruby: x.class; x.is_a?(Integer)
来源：https://mx.zhonguo7118.cn

C#:   x.GetType().Name; x is int
来源：https://mo.zhonguo8118.cn

[A05] 整数除法与取模
来源：https://ly.zhonguo4118.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：https://ye.zhonguo8118.cn

PHP:  intdiv(7, 2); 7 % 2
来源：https://ww.zhonguo2118.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：https://cr.zhonguo2118.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：https://gm.zhonguo7118.cn

Java: 7 / 2; 7 % 2
来源：https://tg.zhonguo6118.cn

Go:   7 / 2; 7 % 2
来源：https://qs.zhonguo1118.cn

Ruby: 7 / 2; 7 % 2
来源：https://zn.zhonguo8118.cn

C#:   7 / 2; 7 % 2
来源：https://kl.zhonguo8118.cn

[A06] 字符串转数字
来源：https://im.zhonguo2118.cn

Py:   int("42"); float("3.14")
来源：https://st.zhonguo6118.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：https://dw.zhonguo7118.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：https://gg.zhonguo4118.cn

TS:   parseInt("42", 10); Number("42")
来源：https://me.zhonguo6118.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：https://xb.zhonguo6118.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：https://zh.zhonguo4118.cn

Ruby: "42".to_i; "3.14".to_f
来源：https://di.zhonguo6118.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：https://ru.zhonguo8118.cn

[A07] 数字转字符串
来源：https://vi.zhonguo2118.cn

Py:   str(42)
来源：https://vw.zhonguo3118.cn

PHP:  (string) 42; strval(42)
来源：https://kn.zhonguo1118.cn

JS:   String(42); (42).toString()
来源：https://dc.zhonguo7118.cn

TS:   String(42)
来源：https://zs.zhonguo5118.cn

Java: String.valueOf(42); Integer.toString(42)
来源：https://iq.zhonguo3118.cn

Go:   strconv.Itoa(42)
来源：https://dl.zhonguo2118.cn

Ruby: 42.to_s
来源：https://xp.zhonguo1118.cn

C#:   42.ToString()
来源：https://zq.zhonguo1118.cn

[A08] 取整与四舍五入
来源：https://vj.zhonguo4118.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：https://ni.zhonguo8118.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：https://fe.zhonguo8118.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：https://qh.zhonguo2118.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：https://xi.zhonguo3118.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：https://hn.zhonguo6118.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：https://jf.zhonguo3118.cn

Ruby: 3.567.round(2); 3.9.floor
来源：https://bz.zhonguo1118.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：https://mf.zhonguo6118.cn

[A09] 绝对值与最大最小值
来源：https://yq.zhonguo7118.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：https://ox.zhonguo8118.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：https://se.zhonguo8118.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：https://je.zhonguo4118.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：https://bp.zhonguo8118.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：https://mr.zhonguo7118.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：https://gq.zhonguo2118.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：https://ru.zhonguo8118.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：https://xu.zhonguo6118.cn

[A10] 生成随机数
来源：https://uz.zhonguo8118.cn

Py:   import random; random.randint(1, 100)
来源：https://db.zhonguo8118.cn

PHP:  random_int(1, 100);
来源：https://uo.zhonguo6118.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：https://km.zhonguo4118.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：https://sf.zhonguo1118.cn

Java: new Random().nextInt(100) + 1
来源：https://xs.zhonguo1118.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：https://px.zhonguo3118.cn

Ruby: rand(1..100)
来源：https://jp.zhonguo5118.cn

C#:   new Random().Next(1, 101)
来源：https://yq.zhonguo1118.cn

[A11] 条件表达式（三元）
来源：https://xs.zhonguo8118.cn

Py:   "yes" if x > 0 else "no"
来源：https://ju.zhonguo3118.cn

PHP:  $x > 0 ? "yes" : "no"
来源：https://zi.zhonguo3118.cn

JS:   x > 0 ? "yes" : "no"
来源：https://ke.zhonguo2118.cn

TS:   x > 0 ? "yes" : "no"
来源：https://ah.zhonguo4118.cn

Java: x > 0 ? "yes" : "no"
来源：https://sl.zhonguo4118.cn

Go:   // 无三元运算符，需用 if 语句
来源：https://ps.zhonguo7118.cn

Ruby: x > 0 ? "yes" : "no"
来源：https://lm.zhonguo5118.cn

C#:   x > 0 ? "yes" : "no"
来源：https://kj.zhonguo8118.cn

[A12] 字符串插值 / 格式化
来源：https://nd.zhonguo6118.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：https://do.zhonguo3118.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：https://wy.zhonguo2118.cn

JS:   `Hello, ${name}!`
来源：https://lp.zhonguo4118.cn

TS:   `Hello, ${name}!`
来源：https://va.zhonguo2118.cn

Java: "Hello, %s!".formatted(name)
来源：https://ol.zhonguo5118.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：https://pr.zhonguo8118.cn

Ruby: "Hello, #{name}!"
来源：https://xq.zhonguo2118.cn

C#:   $"Hello, {name}!"
来源：https://ea.zhonguo8118.cn

[A13] 多行字符串（练习 \n 转义）
来源：https://il.zhonguo8118.cn

Py:   "第一行\n第二行"
来源：https://ln.zhonguo7118.cn

PHP:  "第一行\n第二行"
来源：https://ac.zhonguo7118.cn

JS:   "第一行\n第二行"
来源：https://ve.zhonguo3118.cn

TS:   "第一行\n第二行"
来源：https://gu.zhonguo4118.cn

Java: "第一行\n第二行"
来源：https://dd.zhonguo7118.cn

Go:   "第一行\n第二行"
来源：https://je.zhonguo2118.cn

Ruby: "第一行\n第二行"
来源：https://ef.zhonguo4118.cn

C#:   "第一行\n第二行"
来源：https://kg.zhonguo7118.cn

[A14] 注释写法
来源：https://vf.zhonguo3118.cn

Py:   # 单行；三引号字符串可作多行说明
来源：https://ns.zhonguo5118.cn

PHP:  // 或 # 单行；/* 多行 */
来源：https://io.zhonguo7118.cn

JS:   // 单行；/* 多行 */
来源：https://vn.zhonguo6118.cn

TS:   // 单行；/* 多行 */
来源：https://ng.zhonguo1118.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：https://le.zhonguo5118.cn

Go:   // 单行；/* 多行 */
来源：https://rs.zhonguo1118.cn

Ruby: # 单行；=begin 多行 =end
来源：https://jq.zhonguo6118.cn

C#:   // 单行；/* 多行 */
来源：https://zu.zhonguo1118.cn

[A15] 空值判断与默认值
来源：https://vr.zhonguo6118.cn

Py:   value = data or "默认值"
来源：https://lm.zhonguo1118.cn

PHP:  $value = $data ?? "默认值";
来源：https://dv.zhonguo8118.cn

JS:   const value = data ?? "默认值";
来源：https://cc.zhonguo6118.cn

TS:   const value = data ?? "默认值";
来源：https://al.zhonguo1118.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：https://ez.zhonguo4118.cn

Go:   if data == "" { data = "默认值" }
来源：https://uz.zhonguo6118.cn

Ruby: value = data || "默认值"
来源：https://xb.zhonguo4118.cn

C#:   var value = data ?? "默认值";
来源：https://tk.zhonguo5118.cn

[A16] 真假值判断规则
来源：https://ix.zhonguo7118.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：https://sr.zhonguo7118.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：https://pi.zhonguo7118.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：https://uh.zhonguo6118.cn

TS:   if (!x) {}
来源：https://kj.zhonguo6118.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：https://eg.zhonguo8118.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：https://vi.zhonguo1118.cn

Ruby: unless x            # nil 与 false 为假
来源：https://ip.zhonguo3118.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：https://au.zhonguo3118.cn

[A17] 位运算
来源：https://qu.zhonguo3118.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://yq.zhonguo7118.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：https://mk.zhonguo3118.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://sd.zhonguo1118.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：https://jl.zhonguo1118.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://zt.zhonguo8118.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：https://pq.zhonguo7118.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://ih.zhonguo2118.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://hg.zhonguo2118.cn

[A18] 字符与 ASCII 码互转
来源：https://it.zhonguo5118.cn

Py:   ord("A"); chr(65)
来源：https://wi.zhonguo4118.cn

PHP:  ord("A"); chr(65)
来源：https://bf.zhonguo6118.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：https://my.zhonguo6118.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：https://vt.zhonguo1118.cn

Java: (int) 'A'; (char) 65
来源：https://kj.zhonguo6118.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：https://zn.zhonguo2118.cn

Ruby: "A".ord; 65.chr
来源：https://xn.zhonguo7118.cn

C#:   (int)'A'; (char)65
来源：https://md.zhonguo3118.cn

[A19] 交换两个变量
来源：https://rt.zhonguo6118.cn

Py:   a, b = b, a
来源：https://ve.zhonguo3118.cn

PHP:  [$a, $b] = [$b, $a];
来源：https://fl.zhonguo1118.cn

JS:   [a, b] = [b, a];
来源：https://iy.zhonguo3118.cn

TS:   [a, b] = [b, a];
来源：https://lk.zhonguo7118.cn

Java: int t = a; a = b; b = t;
来源：https://ow.zhonguo8118.cn

Go:   a, b = b, a
来源：https://db.zhonguo3118.cn

Ruby: a, b = b, a
来源：https://op.zhonguo6118.cn

C#:   (a, b) = (b, a);
来源：https://bu.zhonguo6118.cn

[A20] 读取标准输入
来源：https://xs.zhonguo8118.cn

Py:   name = input("请输入：")
来源：https://rc.zhonguo6118.cn

PHP:  $name = trim(fgets(STDIN));
来源：https://nf.zhonguo2118.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：https://et.zhonguo3118.cn

TS:   // Node.js：readline 模块
来源：https://dz.zhonguo7118.cn

Java: new Scanner(System.in).nextLine()
来源：https://ut.zhonguo6118.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：https://vb.zhonguo7118.cn

Ruby: gets.chomp
来源：https://vu.zhonguo7118.cn

C#:   Console.ReadLine();
来源：https://rd.zhonguo8118.cn

[A21] 保留指定小数位输出
来源：https://sa.zhonguo7118.cn

Py:   f"{3.14159:.2f}"
来源：https://ol.zhonguo7118.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：https://lc.zhonguo5118.cn

JS:   (3.14159).toFixed(2)
来源：https://wl.zhonguo4118.cn

TS:   (3.14159).toFixed(2)
来源：https://vv.zhonguo2118.cn

Java: String.format("%.2f", 3.14159)
来源：https://cd.zhonguo4118.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：https://cg.zhonguo2118.cn

Ruby: format("%.2f", 3.14159)
来源：https://js.zhonguo6118.cn

C#:   3.14159.ToString("F2")
来源：https://tl.zhonguo5118.cn

[A22] 获取字符串长度
来源：https://pt.zhonguo8118.cn

Py:   len(s)
来源：https://gr.zhonguo1118.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：https://lf.zhonguo3118.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：https://mx.zhonguo5118.cn

TS:   s.length
来源：https://eb.zhonguo1118.cn

Java: s.length()
来源：https://ql.zhonguo5118.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：https://vc.zhonguo4118.cn

Ruby: s.length
来源：https://jh.zhonguo4118.cn

C#:   s.Length
来源：https://eo.zhonguo1118.cn

[A23] 大小写转换
来源：https://gi.zhonguo3118.cn

Py:   s.upper(); s.lower(); s.title()
来源：https://si.zhonguo4118.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：https://ce.zhonguo5118.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：https://dp.zhonguo4118.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：https://ut.zhonguo5118.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：https://vu.zhonguo4118.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：https://bg.zhonguo3118.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：https://qw.zhonguo7118.cn

C#:   s.ToUpper(); s.ToLower()
来源：https://dr.zhonguo7118.cn

[A24] 去除首尾空白
来源：https://tj.zhonguo4118.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：https://ef.zhonguo4118.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：https://td.zhonguo3118.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://mw.zhonguo5118.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://jr.zhonguo8118.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：https://ex.zhonguo1118.cn

Go:   strings.TrimSpace(s)
来源：https://je.zhonguo5118.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：https://td.zhonguo4118.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：https://qx.zhonguo6118.cn

[A25] 字符串比较
来源：https://rh.zhonguo5118.cn

Py:   s1 == s2; s1 != s2
来源：https://ez.zhonguo2118.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：https://na.zhonguo1118.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：https://zb.zhonguo3118.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：https://pz.zhonguo6118.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：https://dz.zhonguo8118.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：https://ot.zhonguo8118.cn

Ruby: s1 == s2; s1 <=> s2
来源：https://ge.zhonguo2118.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：https://ru.zhonguo4118.cn

[A26] 类型转换总览
来源：https://gu.zhonguo3118.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：https://hb.zhonguo4118.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：https://he.zhonguo3118.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：https://bj.zhonguo7118.cn

TS:   Number() String() Boolean() x as number
来源：https://od.zhonguo4118.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：https://jb.zhonguo1118.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：https://qb.zhonguo1118.cn

Ruby: to_i to_f to_s to_sym to_a
来源：https://ok.zhonguo7118.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：https://ji.zhonguo1118.cn

================================================================================
来源：https://ow.zhonguo2118.cn

B. 流程控制
来源：https://pc.zhonguo5118.cn

================================================================================
来源：https://il.zhonguo2118.cn

[B01] 条件判断 if / else
来源：https://nf.zhonguo2118.cn

Py:   result = "正" if x > 0 else "非正"
来源：https://vo.zhonguo8118.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：https://nh.zhonguo7118.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：https://ac.zhonguo4118.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：https://eb.zhonguo8118.cn

Java: String r = x > 0 ? "正" : "非正";
来源：https://vx.zhonguo1118.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：https://sd.zhonguo3118.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：https://nv.zhonguo6118.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：https://cy.zhonguo6118.cn

[B02] 多分支 else if / elif
来源：https://pi.zhonguo7118.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：https://gc.zhonguo2118.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：https://ds.zhonguo5118.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://tu.zhonguo3118.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://bg.zhonguo4118.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://xu.zhonguo7118.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：https://cq.zhonguo3118.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：https://hc.zhonguo7118.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://lr.zhonguo4118.cn

[B03] switch / match / case
来源：https://pz.zhonguo8118.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：https://gp.zhonguo7118.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：https://fe.zhonguo6118.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://vy.zhonguo3118.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://xd.zhonguo8118.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：https://ip.zhonguo5118.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：https://wy.zhonguo7118.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：https://yz.zhonguo4118.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：https://nr.zhonguo8118.cn

[B04] for 计数循环
来源：https://qd.zhonguo8118.cn

Py:   for i in range(10): print(i)
来源：https://ws.zhonguo5118.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：https://ie.zhonguo7118.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://af.zhonguo2118.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://tg.zhonguo5118.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：https://is.zhonguo8118.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：https://tl.zhonguo7118.cn

Ruby: 10.times { |i| puts i }
来源：https://av.zhonguo7118.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：https://gs.zhonguo3118.cn

[B05] 遍历数组 / 列表
来源：https://rm.zhonguo2118.cn

Py:   for item in arr: print(item)
来源：https://kq.zhonguo1118.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：https://li.zhonguo1118.cn

JS:   for (const item of arr) { console.log(item); }
来源：https://xg.zhonguo6118.cn

TS:   for (const item of arr) { console.log(item); }
来源：https://lo.zhonguo6118.cn

Java: for (var item : arr) { System.out.println(item); }
来源：https://vi.zhonguo1118.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：https://xm.zhonguo4118.cn

Ruby: arr.each { |item| puts item }
来源：https://jg.zhonguo2118.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：https://mn.zhonguo8118.cn

[B06] 遍历字典 / 对象
来源：https://ti.zhonguo2118.cn

Py:   for k, v in d.items(): print(k, v)
来源：https://gv.zhonguo6118.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：https://vy.zhonguo6118.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://fq.zhonguo7118.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://ju.zhonguo4118.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：https://ot.zhonguo3118.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：https://tj.zhonguo3118.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：https://rl.zhonguo2118.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：https://ql.zhonguo5118.cn

[B07] while 循环
来源：https://jo.zhonguo3118.cn

Py:   while i < 10: i += 1
来源：https://vt.zhonguo5118.cn

PHP:  while ($i < 10) { $i++; }
来源：https://zc.zhonguo3118.cn

JS:   while (i < 10) { i++; }
来源：https://cu.zhonguo4118.cn

TS:   while (i < 10) { i++; }
来源：https://xe.zhonguo1118.cn

Java: while (i < 10) { i++; }
来源：https://lo.zhonguo2118.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：https://fg.zhonguo5118.cn

Ruby: while i < 10; i += 1; end
来源：https://dt.zhonguo2118.cn

C#:   while (i < 10) { i++; }
来源：https://lq.zhonguo2118.cn

[B08] do-while（至少执行一次）
来源：https://nm.zhonguo2118.cn

Py:   # 无 do-while：用 while True + break
来源：https://zs.zhonguo1118.cn

PHP:  do { $i++; } while ($i < 10);
来源：https://sv.zhonguo1118.cn

JS:   do { i++; } while (i < 10);
来源：https://li.zhonguo8118.cn

TS:   do { i++; } while (i < 10);
来源：https://iv.zhonguo6118.cn

Java: do { i++; } while (i < 10);
来源：https://xs.zhonguo6118.cn

Go:   for { i++; if i >= 10 { break } }
来源：https://yc.zhonguo7118.cn

Ruby: begin; i += 1; end while i < 10
来源：https://ba.zhonguo1118.cn

C#:   do { i++; } while (i < 10);
来源：https://px.zhonguo3118.cn


<!-- 参考信息 -->