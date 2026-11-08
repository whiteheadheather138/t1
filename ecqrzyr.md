代发 wailian999

Go:   reflect.TypeOf(x).Name()
来源：https://sf.zhonguo4118.cn

Ruby: x.class; x.is_a?(Integer)
来源：https://tt.zhonguo8118.cn

C#:   x.GetType().Name; x is int
来源：https://md.zhonguo6118.cn

[A05] 整数除法与取模
来源：https://ph.zhonguo3118.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：https://ia.zhonguo6118.cn

PHP:  intdiv(7, 2); 7 % 2
来源：https://vf.zhonguo7118.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：https://rw.zhonguo7118.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：https://ya.zhonguo7118.cn

Java: 7 / 2; 7 % 2
来源：https://dr.zhonguo5118.cn

Go:   7 / 2; 7 % 2
来源：https://cu.zhonguo8118.cn

Ruby: 7 / 2; 7 % 2
来源：https://by.zhonguo4118.cn

C#:   7 / 2; 7 % 2
来源：https://bu.zhonguo2118.cn

[A06] 字符串转数字
来源：https://vf.zhonguo7118.cn

Py:   int("42"); float("3.14")
来源：https://kj.zhonguo3118.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：https://tb.zhonguo5118.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：https://cx.zhonguo4118.cn

TS:   parseInt("42", 10); Number("42")
来源：https://vp.zhonguo6118.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：https://wt.zhonguo7118.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：https://gp.zhonguo1118.cn

Ruby: "42".to_i; "3.14".to_f
来源：https://bm.zhonguo5118.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：https://fe.zhonguo6118.cn

[A07] 数字转字符串
来源：https://jf.zhonguo6118.cn

Py:   str(42)
来源：https://dw.zhonguo8118.cn

PHP:  (string) 42; strval(42)
来源：https://lc.zhonguo3118.cn

JS:   String(42); (42).toString()
来源：https://uf.zhonguo5118.cn

TS:   String(42)
来源：https://fy.zhonguo8118.cn

Java: String.valueOf(42); Integer.toString(42)
来源：https://mc.zhonguo5118.cn

Go:   strconv.Itoa(42)
来源：https://gc.zhonguo6118.cn

Ruby: 42.to_s
来源：https://eh.zhonguo1118.cn

C#:   42.ToString()
来源：https://mf.zhonguo1118.cn

[A08] 取整与四舍五入
来源：https://mx.zhonguo7118.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：https://ee.zhonguo4118.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：https://nd.zhonguo4118.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：https://vc.zhonguo5118.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：https://ot.zhonguo2118.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：https://fy.zhonguo4118.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：https://xn.zhonguo4118.cn

Ruby: 3.567.round(2); 3.9.floor
来源：https://sr.zhonguo8118.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：https://zv.zhonguo1118.cn

[A09] 绝对值与最大最小值
来源：https://ph.zhonguo7118.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：https://pk.zhonguo8118.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：https://mw.zhonguo8118.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：https://sv.zhonguo8118.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：https://nr.zhonguo7118.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：https://wa.zhonguo1118.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：https://qq.zhonguo5118.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：https://mm.zhonguo8118.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：https://ty.zhonguo7118.cn

[A10] 生成随机数
来源：https://bi.zhonguo7118.cn

Py:   import random; random.randint(1, 100)
来源：https://py.zhonguo4118.cn

PHP:  random_int(1, 100);
来源：https://jj.zhonguo1118.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：https://uq.zhonguo3118.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：https://tl.zhonguo6118.cn

Java: new Random().nextInt(100) + 1
来源：https://wp.zhonguo5118.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：https://nm.zhonguo5118.cn

Ruby: rand(1..100)
来源：https://re.zhonguo6118.cn

C#:   new Random().Next(1, 101)
来源：https://gl.zhonguo6118.cn

[A11] 条件表达式（三元）
来源：https://xx.zhonguo1118.cn

Py:   "yes" if x > 0 else "no"
来源：https://kc.zhonguo3118.cn

PHP:  $x > 0 ? "yes" : "no"
来源：https://qd.zhonguo7118.cn

JS:   x > 0 ? "yes" : "no"
来源：https://jo.zhonguo3118.cn

TS:   x > 0 ? "yes" : "no"
来源：https://xo.zhonguo1118.cn

Java: x > 0 ? "yes" : "no"
来源：https://bj.zhonguo1118.cn

Go:   // 无三元运算符，需用 if 语句
来源：https://sl.zhonguo1118.cn

Ruby: x > 0 ? "yes" : "no"
来源：https://hi.zhonguo6118.cn

C#:   x > 0 ? "yes" : "no"
来源：https://uf.zhonguo4118.cn

[A12] 字符串插值 / 格式化
来源：https://rq.zhonguo5118.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：https://jc.zhonguo8118.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：https://ue.zhonguo2118.cn

JS:   `Hello, ${name}!`
来源：https://bm.zhonguo2118.cn

TS:   `Hello, ${name}!`
来源：https://aa.zhonguo8118.cn

Java: "Hello, %s!".formatted(name)
来源：https://xp.zhonguo3118.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：https://oh.zhonguo1118.cn

Ruby: "Hello, #{name}!"
来源：https://hy.zhonguo5118.cn

C#:   $"Hello, {name}!"
来源：https://zc.zhonguo8118.cn

[A13] 多行字符串（练习 \n 转义）
来源：https://yy.zhonguo6118.cn

Py:   "第一行\n第二行"
来源：https://yd.zhonguo7118.cn

PHP:  "第一行\n第二行"
来源：https://nd.zhonguo4118.cn

JS:   "第一行\n第二行"
来源：https://wd.zhonguo3118.cn

TS:   "第一行\n第二行"
来源：https://pn.zhonguo7118.cn

Java: "第一行\n第二行"
来源：https://fi.zhonguo1118.cn

Go:   "第一行\n第二行"
来源：https://ud.zhonguo6118.cn

Ruby: "第一行\n第二行"
来源：https://fa.zhonguo5118.cn

C#:   "第一行\n第二行"
来源：https://oy.zhonguo5118.cn

[A14] 注释写法
来源：https://gf.zhonguo6118.cn

Py:   # 单行；三引号字符串可作多行说明
来源：https://bt.zhonguo3118.cn

PHP:  // 或 # 单行；/* 多行 */
来源：https://kn.zhonguo4118.cn

JS:   // 单行；/* 多行 */
来源：https://mv.zhonguo3118.cn

TS:   // 单行；/* 多行 */
来源：https://qi.zhonguo3118.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：https://id.zhonguo2118.cn

Go:   // 单行；/* 多行 */
来源：https://dt.zhonguo6118.cn

Ruby: # 单行；=begin 多行 =end
来源：https://xd.zhonguo5118.cn

C#:   // 单行；/* 多行 */
来源：https://rx.zhonguo7118.cn

[A15] 空值判断与默认值
来源：https://zu.zhonguo4118.cn

Py:   value = data or "默认值"
来源：https://cb.zhonguo8118.cn

PHP:  $value = $data ?? "默认值";
来源：https://mx.zhonguo1118.cn

JS:   const value = data ?? "默认值";
来源：https://ap.zhonguo2118.cn

TS:   const value = data ?? "默认值";
来源：https://jm.zhonguo2118.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：https://ff.zhonguo6118.cn

Go:   if data == "" { data = "默认值" }
来源：https://un.zhonguo6118.cn

Ruby: value = data || "默认值"
来源：https://tx.zhonguo4118.cn

C#:   var value = data ?? "默认值";
来源：https://zb.zhonguo8118.cn

[A16] 真假值判断规则
来源：https://js.zhonguo3118.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：https://fk.zhonguo3118.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：https://tb.zhonguo8118.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：https://yg.zhonguo3118.cn

TS:   if (!x) {}
来源：https://aa.zhonguo1118.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：https://tv.zhonguo4118.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：https://cm.zhonguo3118.cn

Ruby: unless x            # nil 与 false 为假
来源：https://uj.zhonguo3118.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：https://ym.zhonguo5118.cn

[A17] 位运算
来源：https://qh.zhonguo8118.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://sv.zhonguo4118.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：https://ib.zhonguo3118.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://hl.zhonguo3118.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：https://dj.zhonguo8118.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://sm.zhonguo4118.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：https://qo.zhonguo6118.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://pn.zhonguo7118.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://au.zhonguo6118.cn

[A18] 字符与 ASCII 码互转
来源：https://zb.zhonguo1118.cn

Py:   ord("A"); chr(65)
来源：https://fi.zhonguo3118.cn

PHP:  ord("A"); chr(65)
来源：https://xx.zhonguo2118.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：https://jz.zhonguo2118.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：https://jp.zhonguo6118.cn

Java: (int) 'A'; (char) 65
来源：https://xb.zhonguo1118.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：https://sm.zhonguo1118.cn

Ruby: "A".ord; 65.chr
来源：https://tc.zhonguo6118.cn

C#:   (int)'A'; (char)65
来源：https://lo.zhonguo3118.cn

[A19] 交换两个变量
来源：https://ly.zhonguo5118.cn

Py:   a, b = b, a
来源：https://bl.zhonguo2118.cn

PHP:  [$a, $b] = [$b, $a];
来源：https://eb.zhonguo3118.cn

JS:   [a, b] = [b, a];
来源：https://hr.zhonguo1118.cn

TS:   [a, b] = [b, a];
来源：https://my.zhonguo3118.cn

Java: int t = a; a = b; b = t;
来源：https://tr.zhonguo2118.cn

Go:   a, b = b, a
来源：https://pj.zhonguo6118.cn

Ruby: a, b = b, a
来源：https://mv.zhonguo3118.cn

C#:   (a, b) = (b, a);
来源：https://sp.zhonguo8118.cn

[A20] 读取标准输入
来源：https://pn.zhonguo4118.cn

Py:   name = input("请输入：")
来源：https://lo.zhonguo5118.cn

PHP:  $name = trim(fgets(STDIN));
来源：https://oo.zhonguo1118.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：https://be.zhonguo5118.cn

TS:   // Node.js：readline 模块
来源：https://bu.zhonguo7118.cn

Java: new Scanner(System.in).nextLine()
来源：https://tm.zhonguo7118.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：https://ju.zhonguo7118.cn

Ruby: gets.chomp
来源：https://ti.zhonguo1118.cn

C#:   Console.ReadLine();
来源：https://wj.zhonguo4118.cn

[A21] 保留指定小数位输出
来源：https://sc.zhonguo1118.cn

Py:   f"{3.14159:.2f}"
来源：https://rw.zhonguo1118.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：https://ge.zhonguo4118.cn

JS:   (3.14159).toFixed(2)
来源：https://ta.zhonguo8118.cn

TS:   (3.14159).toFixed(2)
来源：https://ve.zhonguo3118.cn

Java: String.format("%.2f", 3.14159)
来源：https://vm.zhonguo1118.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：https://kq.zhonguo8118.cn

Ruby: format("%.2f", 3.14159)
来源：https://zf.zhonguo1118.cn

C#:   3.14159.ToString("F2")
来源：https://bp.zhonguo5118.cn

[A22] 获取字符串长度
来源：https://my.zhonguo2118.cn

Py:   len(s)
来源：https://pw.zhonguo4118.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：https://bo.zhonguo2118.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：https://eu.zhonguo5118.cn

TS:   s.length
来源：https://bh.zhonguo2118.cn

Java: s.length()
来源：https://lg.zhonguo7118.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：https://fg.zhonguo8118.cn

Ruby: s.length
来源：https://jq.zhonguo2118.cn

C#:   s.Length
来源：https://zc.zhonguo5118.cn

[A23] 大小写转换
来源：https://wt.zhonguo4118.cn

Py:   s.upper(); s.lower(); s.title()
来源：https://cg.zhonguo2118.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：https://cj.zhonguo5118.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：https://rj.zhonguo6118.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：https://sk.zhonguo7118.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：https://iu.zhonguo6118.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：https://oe.zhonguo5118.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：https://cv.zhonguo6118.cn

C#:   s.ToUpper(); s.ToLower()
来源：https://dw.zhonguo2118.cn

[A24] 去除首尾空白
来源：https://ic.zhonguo8118.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：https://fx.zhonguo3118.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：https://un.zhonguo5118.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://ex.zhonguo2118.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://ft.zhonguo3118.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：https://vx.zhonguo8118.cn

Go:   strings.TrimSpace(s)
来源：https://en.zhonguo5118.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：https://bl.zhonguo8118.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：https://es.zhonguo5118.cn

[A25] 字符串比较
来源：https://qx.zhonguo2118.cn

Py:   s1 == s2; s1 != s2
来源：https://zq.zhonguo8118.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：https://zf.zhonguo4118.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：https://fk.zhonguo4118.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：https://py.zhonguo4118.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：https://kb.zhonguo2118.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：https://vn.zhonguo8118.cn

Ruby: s1 == s2; s1 <=> s2
来源：https://ym.zhonguo4118.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：https://rv.zhonguo1118.cn

[A26] 类型转换总览
来源：https://rx.zhonguo5118.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：https://iq.zhonguo4118.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：https://ef.zhonguo8118.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：https://bh.zhonguo5118.cn

TS:   Number() String() Boolean() x as number
来源：https://cx.zhonguo2118.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：https://wj.zhonguo2118.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：https://nd.zhonguo3118.cn

Ruby: to_i to_f to_s to_sym to_a
来源：https://it.zhonguo1118.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：https://ki.zhonguo5118.cn

================================================================================
来源：https://hv.zhonguo1118.cn

B. 流程控制
来源：https://cc.zhonguo5118.cn

================================================================================
来源：https://zp.zhonguo4118.cn

[B01] 条件判断 if / else
来源：https://nv.zhonguo6118.cn

Py:   result = "正" if x > 0 else "非正"
来源：https://mf.zhonguo5118.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：https://bt.zhonguo3118.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：https://di.zhonguo7118.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：https://bk.zhonguo6118.cn

Java: String r = x > 0 ? "正" : "非正";
来源：https://wk.zhonguo7118.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：https://bj.zhonguo5118.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：https://in.zhonguo5118.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：https://rp.zhonguo6118.cn

[B02] 多分支 else if / elif
来源：https://vi.zhonguo8118.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：https://zl.zhonguo4118.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：https://xr.zhonguo5118.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://vg.zhonguo5118.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://nh.zhonguo2118.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://zw.zhonguo6118.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：https://eg.zhonguo8118.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：https://yc.zhonguo1118.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://bx.zhonguo6118.cn

[B03] switch / match / case
来源：https://az.zhonguo4118.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：https://ib.zhonguo5118.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：https://al.zhonguo8118.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://ol.zhonguo7118.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://at.zhonguo7118.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：https://aq.zhonguo2118.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：https://pj.zhonguo7118.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：https://jt.zhonguo4118.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：https://kz.zhonguo8118.cn

[B04] for 计数循环
来源：https://mr.zhonguo1118.cn

Py:   for i in range(10): print(i)
来源：https://fv.zhonguo1118.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：https://ku.zhonguo7118.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://yo.zhonguo7118.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://hu.zhonguo8118.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：https://pv.zhonguo7118.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：https://au.zhonguo5118.cn

Ruby: 10.times { |i| puts i }
来源：https://op.zhonguo4118.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：https://ho.zhonguo4118.cn

[B05] 遍历数组 / 列表
来源：https://le.zhonguo8118.cn

Py:   for item in arr: print(item)
来源：https://os.zhonguo2118.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：https://tj.zhonguo8118.cn

JS:   for (const item of arr) { console.log(item); }
来源：https://ig.zhonguo4118.cn

TS:   for (const item of arr) { console.log(item); }
来源：https://dp.zhonguo6118.cn

Java: for (var item : arr) { System.out.println(item); }
来源：https://zb.zhonguo5118.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：https://jh.zhonguo3118.cn

Ruby: arr.each { |item| puts item }
来源：https://io.zhonguo2118.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：https://pw.zhonguo7118.cn

[B06] 遍历字典 / 对象
来源：https://cq.zhonguo3118.cn

Py:   for k, v in d.items(): print(k, v)
来源：https://vu.zhonguo5118.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：https://vd.zhonguo5118.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://zi.zhonguo5118.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://lh.zhonguo6118.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：https://eo.zhonguo3118.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：https://lf.zhonguo1118.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：https://na.zhonguo3118.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：https://gu.zhonguo2118.cn

[B07] while 循环
来源：https://tb.zhonguo1118.cn

Py:   while i < 10: i += 1
来源：https://mr.zhonguo8118.cn

PHP:  while ($i < 10) { $i++; }
来源：https://ti.zhonguo8118.cn

JS:   while (i < 10) { i++; }
来源：https://un.zhonguo7118.cn

TS:   while (i < 10) { i++; }
来源：https://uk.zhonguo7118.cn

Java: while (i < 10) { i++; }
来源：https://wt.zhonguo6118.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：https://iu.zhonguo2118.cn

Ruby: while i < 10; i += 1; end
来源：https://fn.zhonguo2118.cn

C#:   while (i < 10) { i++; }
来源：https://fd.zhonguo4118.cn

[B08] do-while（至少执行一次）
来源：https://fw.zhonguo7118.cn

Py:   # 无 do-while：用 while True + break
来源：https://ya.zhonguo8118.cn

PHP:  do { $i++; } while ($i < 10);
来源：https://ru.zhonguo8118.cn

JS:   do { i++; } while (i < 10);
来源：https://gg.zhonguo2118.cn

TS:   do { i++; } while (i < 10);
来源：https://gs.zhonguo7118.cn

Java: do { i++; } while (i < 10);
来源：https://is.zhonguo5118.cn

Go:   for { i++; if i >= 10 { break } }
来源：https://rh.zhonguo6118.cn

Ruby: begin; i += 1; end while i < 10
来源：https://lk.zhonguo2118.cn

C#:   do { i++; } while (i < 10);
来源：https://ue.zhonguo8118.cn

[B09] break 与 continue
来源：https://xq.zhonguo4118.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：https://uu.zhonguo5118.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：https://sa.zhonguo1118.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://lc.zhonguo1118.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://yb.zhonguo3118.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://kd.zhonguo3118.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：https://dz.zhonguo6118.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：https://gz.zhonguo4118.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://ly.zhonguo2118.cn

[B10] 遍历同时拿索引
来源：https://fq.zhonguo1118.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：https://mg.zhonguo1118.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：https://cn.zhonguo7118.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：https://zd.zhonguo3118.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：https://gk.zhonguo4118.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：https://qb.zhonguo8118.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：https://tt.zhonguo2118.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：https://fu.zhonguo3118.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：https://cu.zhonguo1118.cn

[B11] 生成数字序列 / 区间
来源：https://fi.zhonguo7118.cn

Py:   list(range(0, 10, 2))
来源：https://yv.zhonguo5118.cn

PHP:  range(0, 10, 2);
来源：https://yq.zhonguo7118.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：https://pp.zhonguo6118.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：https://ao.zhonguo1118.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：https://lb.zhonguo5118.cn


<!-- 参考信息 -->