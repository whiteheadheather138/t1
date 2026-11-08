代发 wailian999

Py:   7 // 2   # 3        7 % 2   # 1
来源：https://hf.zhonguo6118.cn

PHP:  intdiv(7, 2); 7 % 2
来源：https://fu.zhonguo5118.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：https://yb.zhonguo4118.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：https://wc.zhonguo4118.cn

Java: 7 / 2; 7 % 2
来源：https://ud.zhonguo5118.cn

Go:   7 / 2; 7 % 2
来源：https://ov.zhonguo5118.cn

Ruby: 7 / 2; 7 % 2
来源：https://op.zhonguo7118.cn

C#:   7 / 2; 7 % 2
来源：https://gd.zhonguo1118.cn

[A06] 字符串转数字
来源：https://qe.zhonguo3118.cn

Py:   int("42"); float("3.14")
来源：https://yx.zhonguo6118.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：https://qx.zhonguo6118.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：https://bo.zhonguo8118.cn

TS:   parseInt("42", 10); Number("42")
来源：https://zc.zhonguo4118.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：https://uk.zhonguo8118.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：https://hg.zhonguo8118.cn

Ruby: "42".to_i; "3.14".to_f
来源：https://zh.zhonguo6118.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：https://dk.zhonguo3118.cn

[A07] 数字转字符串
来源：https://kd.zhonguo5118.cn

Py:   str(42)
来源：https://ef.zhonguo2118.cn

PHP:  (string) 42; strval(42)
来源：https://ax.zhonguo8118.cn

JS:   String(42); (42).toString()
来源：https://hp.zhonguo2118.cn

TS:   String(42)
来源：https://mq.zhonguo1118.cn

Java: String.valueOf(42); Integer.toString(42)
来源：https://zw.zhonguo5118.cn

Go:   strconv.Itoa(42)
来源：https://xd.zhonguo6118.cn

Ruby: 42.to_s
来源：https://if.zhonguo4118.cn

C#:   42.ToString()
来源：https://dq.zhonguo3118.cn

[A08] 取整与四舍五入
来源：https://za.zhonguo8118.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：https://jn.zhonguo7118.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：https://mx.zhonguo1118.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：https://fj.zhonguo4118.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：https://iw.zhonguo8118.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：https://xb.zhonguo1118.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：https://du.zhonguo4118.cn

Ruby: 3.567.round(2); 3.9.floor
来源：https://lw.zhonguo1118.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：https://cv.zhonguo5118.cn

[A09] 绝对值与最大最小值
来源：https://fl.zhonguo7118.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：https://gj.zhonguo8118.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：https://ct.zhonguo8118.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：https://dg.zhonguo3118.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：https://pc.zhonguo6118.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：https://mr.zhonguo6118.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：https://ye.zhonguo4118.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：https://gd.zhonguo3118.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：https://gm.zhonguo2118.cn

[A10] 生成随机数
来源：https://ht.zhonguo3118.cn

Py:   import random; random.randint(1, 100)
来源：https://pg.zhonguo1118.cn

PHP:  random_int(1, 100);
来源：https://sl.zhonguo3118.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：https://gs.zhonguo5118.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：https://km.zhonguo1118.cn

Java: new Random().nextInt(100) + 1
来源：https://sf.zhonguo3118.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：https://no.zhonguo5118.cn

Ruby: rand(1..100)
来源：https://xg.zhonguo7118.cn

C#:   new Random().Next(1, 101)
来源：https://cb.zhonguo5118.cn

[A11] 条件表达式（三元）
来源：https://xv.zhonguo8118.cn

Py:   "yes" if x > 0 else "no"
来源：https://vb.zhonguo8118.cn

PHP:  $x > 0 ? "yes" : "no"
来源：https://co.zhonguo7118.cn

JS:   x > 0 ? "yes" : "no"
来源：https://am.zhonguo5118.cn

TS:   x > 0 ? "yes" : "no"
来源：https://py.zhonguo4118.cn

Java: x > 0 ? "yes" : "no"
来源：https://iz.zhonguo4118.cn

Go:   // 无三元运算符，需用 if 语句
来源：https://jh.zhonguo5118.cn

Ruby: x > 0 ? "yes" : "no"
来源：https://vd.zhonguo6118.cn

C#:   x > 0 ? "yes" : "no"
来源：https://tf.zhonguo8118.cn

[A12] 字符串插值 / 格式化
来源：https://rl.zhonguo8118.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：https://xq.zhonguo8118.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：https://uk.zhonguo4118.cn

JS:   `Hello, ${name}!`
来源：https://gh.zhonguo8118.cn

TS:   `Hello, ${name}!`
来源：https://fn.zhonguo5118.cn

Java: "Hello, %s!".formatted(name)
来源：https://kv.zhonguo2118.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：https://nq.zhonguo6118.cn

Ruby: "Hello, #{name}!"
来源：https://rd.zhonguo3118.cn

C#:   $"Hello, {name}!"
来源：https://sh.zhonguo8118.cn

[A13] 多行字符串（练习 \n 转义）
来源：https://da.zhonguo4118.cn

Py:   "第一行\n第二行"
来源：https://ik.zhonguo4118.cn

PHP:  "第一行\n第二行"
来源：https://is.zhonguo2118.cn

JS:   "第一行\n第二行"
来源：https://zx.zhonguo4118.cn

TS:   "第一行\n第二行"
来源：https://hf.zhonguo8118.cn

Java: "第一行\n第二行"
来源：https://fy.zhonguo6118.cn

Go:   "第一行\n第二行"
来源：https://ed.zhonguo6118.cn

Ruby: "第一行\n第二行"
来源：https://ln.zhonguo1118.cn

C#:   "第一行\n第二行"
来源：https://xg.zhonguo6118.cn

[A14] 注释写法
来源：https://ts.zhonguo2118.cn

Py:   # 单行；三引号字符串可作多行说明
来源：https://fq.zhonguo1118.cn

PHP:  // 或 # 单行；/* 多行 */
来源：https://gz.zhonguo6118.cn

JS:   // 单行；/* 多行 */
来源：https://vu.zhonguo2118.cn

TS:   // 单行；/* 多行 */
来源：https://wv.zhonguo2118.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：https://qp.zhonguo8118.cn

Go:   // 单行；/* 多行 */
来源：https://tl.zhonguo1118.cn

Ruby: # 单行；=begin 多行 =end
来源：https://ct.zhonguo5118.cn

C#:   // 单行；/* 多行 */
来源：https://tx.zhonguo8118.cn

[A15] 空值判断与默认值
来源：https://el.zhonguo1118.cn

Py:   value = data or "默认值"
来源：https://sx.zhonguo8118.cn

PHP:  $value = $data ?? "默认值";
来源：https://cf.zhonguo3118.cn

JS:   const value = data ?? "默认值";
来源：https://da.zhonguo1118.cn

TS:   const value = data ?? "默认值";
来源：https://mp.zhonguo3118.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：https://sw.zhonguo5118.cn

Go:   if data == "" { data = "默认值" }
来源：https://tk.zhonguo6118.cn

Ruby: value = data || "默认值"
来源：https://tv.zhonguo3118.cn

C#:   var value = data ?? "默认值";
来源：https://lm.zhonguo5118.cn

[A16] 真假值判断规则
来源：https://zn.zhonguo6118.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：https://ju.zhonguo5118.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：https://do.zhonguo3118.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：https://uj.zhonguo7118.cn

TS:   if (!x) {}
来源：https://po.zhonguo1118.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：https://jc.zhonguo6118.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：https://gr.zhonguo7118.cn

Ruby: unless x            # nil 与 false 为假
来源：https://ha.zhonguo2118.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：https://wz.zhonguo4118.cn

[A17] 位运算
来源：https://aw.zhonguo4118.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://gi.zhonguo3118.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：https://ry.zhonguo6118.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://fz.zhonguo2118.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：https://gc.zhonguo2118.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://ja.zhonguo1118.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：https://qc.zhonguo8118.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://an.zhonguo5118.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://zk.zhonguo1118.cn

[A18] 字符与 ASCII 码互转
来源：https://zd.zhonguo6118.cn

Py:   ord("A"); chr(65)
来源：https://id.zhonguo1118.cn

PHP:  ord("A"); chr(65)
来源：https://gr.zhonguo4118.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：https://mi.zhonguo5118.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：https://ac.zhonguo7118.cn

Java: (int) 'A'; (char) 65
来源：https://em.zhonguo5118.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：https://hv.zhonguo2118.cn

Ruby: "A".ord; 65.chr
来源：https://vf.zhonguo6118.cn

C#:   (int)'A'; (char)65
来源：https://ie.zhonguo5118.cn

[A19] 交换两个变量
来源：https://vh.zhonguo2118.cn

Py:   a, b = b, a
来源：https://un.zhonguo6118.cn

PHP:  [$a, $b] = [$b, $a];
来源：https://ff.zhonguo7118.cn

JS:   [a, b] = [b, a];
来源：https://rg.zhonguo4118.cn

TS:   [a, b] = [b, a];
来源：https://bm.zhonguo5118.cn

Java: int t = a; a = b; b = t;
来源：https://qf.zhonguo1118.cn

Go:   a, b = b, a
来源：https://ha.zhonguo2118.cn

Ruby: a, b = b, a
来源：https://fv.zhonguo4118.cn

C#:   (a, b) = (b, a);
来源：https://sx.zhonguo1118.cn

[A20] 读取标准输入
来源：https://eg.zhonguo4118.cn

Py:   name = input("请输入：")
来源：https://ua.zhonguo2118.cn

PHP:  $name = trim(fgets(STDIN));
来源：https://yf.zhonguo4118.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：https://fj.zhonguo2118.cn

TS:   // Node.js：readline 模块
来源：https://op.zhonguo8118.cn

Java: new Scanner(System.in).nextLine()
来源：https://wk.zhonguo2118.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：https://kt.zhonguo8118.cn

Ruby: gets.chomp
来源：https://mf.zhonguo2118.cn

C#:   Console.ReadLine();
来源：https://im.zhonguo6118.cn

[A21] 保留指定小数位输出
来源：https://ic.zhonguo3118.cn

Py:   f"{3.14159:.2f}"
来源：https://eb.zhonguo5118.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：https://nx.zhonguo6118.cn

JS:   (3.14159).toFixed(2)
来源：https://ua.zhonguo5118.cn

TS:   (3.14159).toFixed(2)
来源：https://ra.zhonguo8118.cn

Java: String.format("%.2f", 3.14159)
来源：https://gq.zhonguo6118.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：https://nx.zhonguo5118.cn

Ruby: format("%.2f", 3.14159)
来源：https://ie.zhonguo5118.cn

C#:   3.14159.ToString("F2")
来源：https://zu.zhonguo2118.cn

[A22] 获取字符串长度
来源：https://ds.zhonguo2118.cn

Py:   len(s)
来源：https://zb.zhonguo7118.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：https://uk.zhonguo3118.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：https://rj.zhonguo4118.cn

TS:   s.length
来源：https://pt.zhonguo4118.cn

Java: s.length()
来源：https://gv.zhonguo6118.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：https://wc.zhonguo8118.cn

Ruby: s.length
来源：https://er.zhonguo1118.cn

C#:   s.Length
来源：https://yk.zhonguo3118.cn

[A23] 大小写转换
来源：https://tk.zhonguo3118.cn

Py:   s.upper(); s.lower(); s.title()
来源：https://it.zhonguo7118.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：https://ob.zhonguo8118.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：https://op.zhonguo7118.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：https://gv.zhonguo3118.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：https://nf.zhonguo6118.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：https://fz.zhonguo1118.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：https://dw.zhonguo7118.cn

C#:   s.ToUpper(); s.ToLower()
来源：https://ie.zhonguo8118.cn

[A24] 去除首尾空白
来源：https://tb.zhonguo2118.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：https://so.zhonguo1118.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：https://ia.zhonguo6118.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://le.zhonguo3118.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://fx.zhonguo5118.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：https://de.zhonguo1118.cn

Go:   strings.TrimSpace(s)
来源：https://tb.zhonguo5118.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：https://uy.zhonguo5118.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：https://ey.zhonguo6118.cn

[A25] 字符串比较
来源：https://iy.zhonguo7118.cn

Py:   s1 == s2; s1 != s2
来源：https://yv.zhonguo1118.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：https://gm.zhonguo1118.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：https://uy.zhonguo5118.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：https://ol.zhonguo4118.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：https://ta.zhonguo8118.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：https://yt.zhonguo6118.cn

Ruby: s1 == s2; s1 <=> s2
来源：https://is.zhonguo8118.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：https://zj.zhonguo6118.cn

[A26] 类型转换总览
来源：https://wh.zhonguo1118.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：https://ee.zhonguo4118.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：https://oj.zhonguo7118.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：https://gu.zhonguo1118.cn

TS:   Number() String() Boolean() x as number
来源：https://fj.zhonguo2118.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：https://lo.zhonguo4118.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：https://nn.zhonguo3118.cn

Ruby: to_i to_f to_s to_sym to_a
来源：https://eg.zhonguo7118.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：https://yk.zhonguo1118.cn

================================================================================
来源：https://js.zhonguo1118.cn

B. 流程控制
来源：https://yp.zhonguo7118.cn

================================================================================
来源：https://vz.zhonguo6118.cn

[B01] 条件判断 if / else
来源：https://cb.zhonguo7118.cn

Py:   result = "正" if x > 0 else "非正"
来源：https://bu.zhonguo2118.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：https://qo.zhonguo1118.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：https://po.zhonguo6118.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：https://yi.zhonguo5118.cn

Java: String r = x > 0 ? "正" : "非正";
来源：https://xp.zhonguo3118.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：https://ej.zhonguo7118.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：https://nf.zhonguo8118.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：https://ft.zhonguo4118.cn

[B02] 多分支 else if / elif
来源：https://yw.zhonguo4118.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：https://gb.zhonguo5118.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：https://og.zhonguo4118.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://zo.zhonguo7118.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://bx.zhonguo3118.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://st.zhonguo2118.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：https://om.zhonguo8118.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：https://zx.zhonguo5118.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://gy.zhonguo3118.cn

[B03] switch / match / case
来源：https://nq.zhonguo8118.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：https://wa.zhonguo1118.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：https://wz.zhonguo7118.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://yj.zhonguo4118.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://rx.zhonguo7118.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：https://zh.zhonguo3118.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：https://pe.zhonguo3118.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：https://vv.zhonguo5118.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：https://at.zhonguo3118.cn

[B04] for 计数循环
来源：https://dt.zhonguo3118.cn

Py:   for i in range(10): print(i)
来源：https://ln.zhonguo5118.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：https://zd.zhonguo1118.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://fn.zhonguo1118.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://ad.zhonguo2118.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：https://jd.zhonguo1118.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：https://lu.zhonguo3118.cn

Ruby: 10.times { |i| puts i }
来源：https://gz.zhonguo8118.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：https://nx.zhonguo6118.cn

[B05] 遍历数组 / 列表
来源：https://wm.zhonguo4118.cn

Py:   for item in arr: print(item)
来源：https://io.zhonguo7118.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：https://ik.zhonguo4118.cn

JS:   for (const item of arr) { console.log(item); }
来源：https://rs.zhonguo4118.cn

TS:   for (const item of arr) { console.log(item); }
来源：https://ol.zhonguo4118.cn

Java: for (var item : arr) { System.out.println(item); }
来源：https://gu.zhonguo5118.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：https://sa.zhonguo1118.cn

Ruby: arr.each { |item| puts item }
来源：https://lu.zhonguo3118.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：https://gk.zhonguo2118.cn

[B06] 遍历字典 / 对象
来源：https://yj.zhonguo3118.cn

Py:   for k, v in d.items(): print(k, v)
来源：https://ed.zhonguo2118.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：https://yu.zhonguo6118.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://ia.zhonguo6118.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://sj.zhonguo5118.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：https://ja.zhonguo4118.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：https://ap.zhonguo4118.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：https://na.zhonguo4118.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：https://ao.zhonguo5118.cn

[B07] while 循环
来源：https://iw.zhonguo6118.cn

Py:   while i < 10: i += 1
来源：https://az.zhonguo2118.cn

PHP:  while ($i < 10) { $i++; }
来源：https://cp.zhonguo4118.cn

JS:   while (i < 10) { i++; }
来源：https://aw.zhonguo7118.cn

TS:   while (i < 10) { i++; }
来源：https://bz.zhonguo6118.cn

Java: while (i < 10) { i++; }
来源：https://kl.zhonguo7118.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：https://jm.zhonguo4118.cn

Ruby: while i < 10; i += 1; end
来源：https://iy.zhonguo8118.cn

C#:   while (i < 10) { i++; }
来源：https://jy.zhonguo3118.cn

[B08] do-while（至少执行一次）
来源：https://fh.zhonguo6118.cn

Py:   # 无 do-while：用 while True + break
来源：https://mk.zhonguo6118.cn

PHP:  do { $i++; } while ($i < 10);
来源：https://me.zhonguo8118.cn

JS:   do { i++; } while (i < 10);
来源：https://az.zhonguo8118.cn

TS:   do { i++; } while (i < 10);
来源：https://ah.zhonguo6118.cn

Java: do { i++; } while (i < 10);
来源：https://yp.zhonguo5118.cn

Go:   for { i++; if i >= 10 { break } }
来源：https://bw.zhonguo4118.cn

Ruby: begin; i += 1; end while i < 10
来源：https://az.zhonguo7118.cn

C#:   do { i++; } while (i < 10);
来源：https://ah.zhonguo5118.cn

[B09] break 与 continue
来源：https://xz.zhonguo1118.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：https://az.zhonguo3118.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：https://gx.zhonguo3118.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://vn.zhonguo7118.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://bs.zhonguo2118.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://nn.zhonguo3118.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：https://ek.zhonguo1118.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：https://nu.zhonguo5118.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://fx.zhonguo6118.cn

[B10] 遍历同时拿索引
来源：https://ne.zhonguo4118.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：https://xs.zhonguo7118.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：https://ac.zhonguo2118.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：https://vv.zhonguo6118.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：https://hx.zhonguo1118.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：https://jr.zhonguo7118.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：https://hn.zhonguo1118.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：https://rz.zhonguo4118.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：https://ht.zhonguo8118.cn

[B11] 生成数字序列 / 区间
来源：https://lo.zhonguo3118.cn

Py:   list(range(0, 10, 2))
来源：https://lo.zhonguo3118.cn

PHP:  range(0, 10, 2);
来源：https://hg.zhonguo4118.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：https://sd.zhonguo5118.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：https://pa.zhonguo1118.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：https://fy.zhonguo4118.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：https://qr.zhonguo3118.cn

Ruby: (0...10).step(2).to_a
来源：https://ru.zhonguo6118.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：https://hv.zhonguo4118.cn

[B12] 跳出多层循环
来源：https://by.zhonguo1118.cn


<!-- 参考信息 -->