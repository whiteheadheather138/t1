代发 wailian999

PHP:  gettype($x); is_int($x); is_string($x)
来源：https://sp.zhonguo3118.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：https://nm.zhonguo5118.cn

TS:   typeof x; x instanceof Date
来源：https://tz.zhonguo8118.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：https://vq.zhonguo5118.cn

Go:   reflect.TypeOf(x).Name()
来源：https://aw.zhonguo2118.cn

Ruby: x.class; x.is_a?(Integer)
来源：https://nd.zhonguo8118.cn

C#:   x.GetType().Name; x is int
来源：https://ba.zhonguo3118.cn

[A05] 整数除法与取模
来源：https://en.zhonguo7118.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：https://ok.zhonguo4118.cn

PHP:  intdiv(7, 2); 7 % 2
来源：https://kz.zhonguo3118.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：https://li.zhonguo3118.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：https://ww.zhonguo7118.cn

Java: 7 / 2; 7 % 2
来源：https://vl.zhonguo2118.cn

Go:   7 / 2; 7 % 2
来源：https://yw.zhonguo5118.cn

Ruby: 7 / 2; 7 % 2
来源：https://ch.zhonguo1118.cn

C#:   7 / 2; 7 % 2
来源：https://gg.zhonguo3118.cn

[A06] 字符串转数字
来源：https://fx.zhonguo8118.cn

Py:   int("42"); float("3.14")
来源：https://qp.zhonguo7118.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：https://ad.zhonguo1118.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：https://pe.zhonguo8118.cn

TS:   parseInt("42", 10); Number("42")
来源：https://lq.zhonguo3118.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：https://cv.zhonguo7118.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：https://zj.zhonguo6118.cn

Ruby: "42".to_i; "3.14".to_f
来源：https://am.zhonguo8118.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：https://vm.zhonguo8118.cn

[A07] 数字转字符串
来源：https://cw.zhonguo7118.cn

Py:   str(42)
来源：https://yl.zhonguo6118.cn

PHP:  (string) 42; strval(42)
来源：https://xb.zhonguo5118.cn

JS:   String(42); (42).toString()
来源：https://xd.zhonguo5118.cn

TS:   String(42)
来源：https://ro.zhonguo4118.cn

Java: String.valueOf(42); Integer.toString(42)
来源：https://rz.zhonguo5118.cn

Go:   strconv.Itoa(42)
来源：https://hc.zhonguo6118.cn

Ruby: 42.to_s
来源：https://vq.zhonguo3118.cn

C#:   42.ToString()
来源：https://ez.zhonguo5118.cn

[A08] 取整与四舍五入
来源：https://tw.zhonguo3118.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：https://wq.zhonguo2118.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：https://cx.zhonguo5118.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：https://nq.zhonguo4118.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：https://nd.zhonguo6118.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：https://ee.zhonguo1118.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：https://jq.zhonguo5118.cn

Ruby: 3.567.round(2); 3.9.floor
来源：https://bg.zhonguo3118.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：https://fm.zhonguo3118.cn

[A09] 绝对值与最大最小值
来源：https://ci.zhonguo3118.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：https://qp.zhonguo6118.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：https://vk.zhonguo5118.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：https://de.zhonguo5118.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：https://tc.zhonguo3118.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：https://hy.zhonguo4118.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：https://uy.zhonguo3118.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：https://zf.zhonguo1118.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：https://tl.zhonguo7118.cn

[A10] 生成随机数
来源：https://bq.zhonguo2118.cn

Py:   import random; random.randint(1, 100)
来源：https://lz.zhonguo5118.cn

PHP:  random_int(1, 100);
来源：https://so.zhonguo8118.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：https://kj.zhonguo4118.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：https://st.zhonguo8118.cn

Java: new Random().nextInt(100) + 1
来源：https://vu.zhonguo1118.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：https://dq.zhonguo2118.cn

Ruby: rand(1..100)
来源：https://gi.zhonguo1118.cn

C#:   new Random().Next(1, 101)
来源：https://hx.zhonguo4118.cn

[A11] 条件表达式（三元）
来源：https://rd.zhonguo1118.cn

Py:   "yes" if x > 0 else "no"
来源：https://zx.zhonguo5118.cn

PHP:  $x > 0 ? "yes" : "no"
来源：https://hm.zhonguo8118.cn

JS:   x > 0 ? "yes" : "no"
来源：https://xg.zhonguo6118.cn

TS:   x > 0 ? "yes" : "no"
来源：https://fe.zhonguo3118.cn

Java: x > 0 ? "yes" : "no"
来源：https://gl.zhonguo7118.cn

Go:   // 无三元运算符，需用 if 语句
来源：https://ab.zhonguo8118.cn

Ruby: x > 0 ? "yes" : "no"
来源：https://nj.zhonguo6118.cn

C#:   x > 0 ? "yes" : "no"
来源：https://gg.zhonguo7118.cn

[A12] 字符串插值 / 格式化
来源：https://ra.zhonguo2118.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：https://xz.zhonguo2118.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：https://iy.zhonguo8118.cn

JS:   `Hello, ${name}!`
来源：https://vc.zhonguo1118.cn

TS:   `Hello, ${name}!`
来源：https://pv.zhonguo1118.cn

Java: "Hello, %s!".formatted(name)
来源：https://tc.zhonguo2118.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：https://sc.zhonguo5118.cn

Ruby: "Hello, #{name}!"
来源：https://ek.zhonguo8118.cn

C#:   $"Hello, {name}!"
来源：https://eb.zhonguo8118.cn

[A13] 多行字符串（练习 \n 转义）
来源：https://rg.zhonguo7118.cn

Py:   "第一行\n第二行"
来源：https://vx.zhonguo3118.cn

PHP:  "第一行\n第二行"
来源：https://yb.zhonguo2118.cn

JS:   "第一行\n第二行"
来源：https://kb.zhonguo7118.cn

TS:   "第一行\n第二行"
来源：https://sh.zhonguo2118.cn

Java: "第一行\n第二行"
来源：https://gn.zhonguo1118.cn

Go:   "第一行\n第二行"
来源：https://cp.zhonguo1118.cn

Ruby: "第一行\n第二行"
来源：https://id.zhonguo6118.cn

C#:   "第一行\n第二行"
来源：https://iq.zhonguo3118.cn

[A14] 注释写法
来源：https://dx.zhonguo7118.cn

Py:   # 单行；三引号字符串可作多行说明
来源：https://hf.zhonguo6118.cn

PHP:  // 或 # 单行；/* 多行 */
来源：https://di.zhonguo1118.cn

JS:   // 单行；/* 多行 */
来源：https://mw.zhonguo7118.cn

TS:   // 单行；/* 多行 */
来源：https://qx.zhonguo6118.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：https://df.zhonguo4118.cn

Go:   // 单行；/* 多行 */
来源：https://rn.zhonguo3118.cn

Ruby: # 单行；=begin 多行 =end
来源：https://ec.zhonguo2118.cn

C#:   // 单行；/* 多行 */
来源：https://eh.zhonguo6118.cn

[A15] 空值判断与默认值
来源：https://rk.zhonguo5118.cn

Py:   value = data or "默认值"
来源：https://cw.zhonguo1118.cn

PHP:  $value = $data ?? "默认值";
来源：https://uv.zhonguo3118.cn

JS:   const value = data ?? "默认值";
来源：https://no.zhonguo5118.cn

TS:   const value = data ?? "默认值";
来源：https://hu.zhonguo3118.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：https://fb.zhonguo6118.cn

Go:   if data == "" { data = "默认值" }
来源：https://tc.zhonguo8118.cn

Ruby: value = data || "默认值"
来源：https://yu.zhonguo3118.cn

C#:   var value = data ?? "默认值";
来源：https://lt.zhonguo6118.cn

[A16] 真假值判断规则
来源：https://pr.zhonguo4118.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：https://nn.zhonguo6118.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：https://tk.zhonguo3118.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：https://ov.zhonguo4118.cn

TS:   if (!x) {}
来源：https://yi.zhonguo3118.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：https://mn.zhonguo6118.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：https://fz.zhonguo6118.cn

Ruby: unless x            # nil 与 false 为假
来源：https://la.zhonguo5118.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：https://xp.zhonguo6118.cn

[A17] 位运算
来源：https://bb.zhonguo1118.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://bn.zhonguo6118.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：https://au.zhonguo5118.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://vy.zhonguo7118.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：https://ht.zhonguo1118.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://jb.zhonguo6118.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：https://mo.zhonguo5118.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://rn.zhonguo6118.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://et.zhonguo1118.cn

[A18] 字符与 ASCII 码互转
来源：https://iq.zhonguo6118.cn

Py:   ord("A"); chr(65)
来源：https://ij.zhonguo8118.cn

PHP:  ord("A"); chr(65)
来源：https://dn.zhonguo8118.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：https://bv.zhonguo6118.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：https://xn.zhonguo8118.cn

Java: (int) 'A'; (char) 65
来源：https://vc.zhonguo3118.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：https://qj.zhonguo5118.cn

Ruby: "A".ord; 65.chr
来源：https://wr.zhonguo2118.cn

C#:   (int)'A'; (char)65
来源：https://py.zhonguo3118.cn

[A19] 交换两个变量
来源：https://gn.zhonguo2118.cn

Py:   a, b = b, a
来源：https://fp.zhonguo3118.cn

PHP:  [$a, $b] = [$b, $a];
来源：https://ra.zhonguo1118.cn

JS:   [a, b] = [b, a];
来源：https://pl.zhonguo6118.cn

TS:   [a, b] = [b, a];
来源：https://eg.zhonguo6118.cn

Java: int t = a; a = b; b = t;
来源：https://ld.zhonguo4118.cn

Go:   a, b = b, a
来源：https://iu.zhonguo2118.cn

Ruby: a, b = b, a
来源：https://mo.zhonguo7118.cn

C#:   (a, b) = (b, a);
来源：https://hl.zhonguo8118.cn

[A20] 读取标准输入
来源：https://hh.zhonguo5118.cn

Py:   name = input("请输入：")
来源：https://hq.zhonguo4118.cn

PHP:  $name = trim(fgets(STDIN));
来源：https://er.zhonguo5118.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：https://ho.zhonguo8118.cn

TS:   // Node.js：readline 模块
来源：https://bf.zhonguo8118.cn

Java: new Scanner(System.in).nextLine()
来源：https://ls.zhonguo7118.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：https://zh.zhonguo5118.cn

Ruby: gets.chomp
来源：https://zw.zhonguo5118.cn

C#:   Console.ReadLine();
来源：https://jt.zhonguo3118.cn

[A21] 保留指定小数位输出
来源：https://jp.zhonguo6118.cn

Py:   f"{3.14159:.2f}"
来源：https://mb.zhonguo7118.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：https://bo.zhonguo7118.cn

JS:   (3.14159).toFixed(2)
来源：https://vl.zhonguo3118.cn

TS:   (3.14159).toFixed(2)
来源：https://rf.zhonguo2118.cn

Java: String.format("%.2f", 3.14159)
来源：https://uq.zhonguo6118.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：https://nv.zhonguo4118.cn

Ruby: format("%.2f", 3.14159)
来源：https://zn.zhonguo6118.cn

C#:   3.14159.ToString("F2")
来源：https://vm.zhonguo7118.cn

[A22] 获取字符串长度
来源：https://hv.zhonguo1118.cn

Py:   len(s)
来源：https://nm.zhonguo6118.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：https://pr.zhonguo4118.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：https://nu.zhonguo3118.cn

TS:   s.length
来源：https://rq.zhonguo4118.cn

Java: s.length()
来源：https://gc.zhonguo3118.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：https://vv.zhonguo5118.cn

Ruby: s.length
来源：https://ao.zhonguo5118.cn

C#:   s.Length
来源：https://yj.zhonguo3118.cn

[A23] 大小写转换
来源：https://bq.zhonguo1118.cn

Py:   s.upper(); s.lower(); s.title()
来源：https://dl.zhonguo1118.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：https://es.zhonguo2118.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：https://bp.zhonguo4118.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：https://ru.zhonguo6118.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：https://fq.zhonguo6118.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：https://yn.zhonguo3118.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：https://zt.zhonguo4118.cn

C#:   s.ToUpper(); s.ToLower()
来源：https://lw.zhonguo6118.cn

[A24] 去除首尾空白
来源：https://cc.zhonguo1118.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：https://kr.zhonguo6118.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：https://gf.zhonguo6118.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://ko.zhonguo1118.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://mn.zhonguo2118.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：https://fv.zhonguo8118.cn

Go:   strings.TrimSpace(s)
来源：https://fa.zhonguo7118.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：https://ku.zhonguo8118.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：https://ka.zhonguo7118.cn

[A25] 字符串比较
来源：https://nz.zhonguo5118.cn

Py:   s1 == s2; s1 != s2
来源：https://ul.zhonguo8118.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：https://oi.zhonguo5118.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：https://wf.zhonguo1118.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：https://ue.zhonguo2118.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：https://je.zhonguo6118.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：https://iz.zhonguo4118.cn

Ruby: s1 == s2; s1 <=> s2
来源：https://vt.zhonguo7118.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：https://rg.zhonguo4118.cn

[A26] 类型转换总览
来源：https://zw.zhonguo4118.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：https://io.zhonguo8118.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：https://xf.zhonguo6118.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：https://wm.zhonguo7118.cn

TS:   Number() String() Boolean() x as number
来源：https://vv.zhonguo6118.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：https://bv.zhonguo4118.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：https://va.zhonguo1118.cn

Ruby: to_i to_f to_s to_sym to_a
来源：https://ud.zhonguo7118.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：https://ge.zhonguo5118.cn

================================================================================
来源：https://jt.zhonguo2118.cn

B. 流程控制
来源：https://in.zhonguo2118.cn

================================================================================
来源：https://gi.zhonguo3118.cn

[B01] 条件判断 if / else
来源：https://ze.zhonguo6118.cn

Py:   result = "正" if x > 0 else "非正"
来源：https://en.zhonguo3118.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：https://xo.zhonguo7118.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：https://wx.zhonguo8118.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：https://eq.zhonguo4118.cn

Java: String r = x > 0 ? "正" : "非正";
来源：https://zm.zhonguo1118.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：https://ws.zhonguo6118.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：https://kp.zhonguo1118.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：https://ui.zhonguo2118.cn

[B02] 多分支 else if / elif
来源：https://fx.zhonguo2118.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：https://wk.zhonguo2118.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：https://ze.zhonguo8118.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://iw.zhonguo2118.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://eq.zhonguo4118.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://bm.zhonguo5118.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：https://uc.zhonguo8118.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：https://md.zhonguo6118.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://di.zhonguo6118.cn

[B03] switch / match / case
来源：https://gx.zhonguo7118.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：https://ea.zhonguo4118.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：https://fd.zhonguo3118.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://jo.zhonguo7118.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://nd.zhonguo3118.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：https://wf.zhonguo8118.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：https://us.zhonguo3118.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：https://uc.zhonguo4118.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：https://pr.zhonguo6118.cn

[B04] for 计数循环
来源：https://kw.zhonguo8118.cn

Py:   for i in range(10): print(i)
来源：https://er.zhonguo3118.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：https://na.zhonguo3118.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://tc.zhonguo5118.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://um.zhonguo5118.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：https://oq.zhonguo3118.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：https://ix.zhonguo3118.cn

Ruby: 10.times { |i| puts i }
来源：https://ua.zhonguo2118.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：https://az.zhonguo8118.cn

[B05] 遍历数组 / 列表
来源：https://rl.zhonguo2118.cn

Py:   for item in arr: print(item)
来源：https://ax.zhonguo5118.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：https://fk.zhonguo7118.cn

JS:   for (const item of arr) { console.log(item); }
来源：https://in.zhonguo8118.cn

TS:   for (const item of arr) { console.log(item); }
来源：https://qh.zhonguo8118.cn

Java: for (var item : arr) { System.out.println(item); }
来源：https://gn.zhonguo8118.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：https://qa.zhonguo6118.cn

Ruby: arr.each { |item| puts item }
来源：https://gr.zhonguo7118.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：https://ew.zhonguo8118.cn

[B06] 遍历字典 / 对象
来源：https://lh.zhonguo3118.cn

Py:   for k, v in d.items(): print(k, v)
来源：https://yh.zhonguo8118.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：https://ml.zhonguo6118.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://vt.zhonguo2118.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://mw.zhonguo3118.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：https://uc.zhonguo1118.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：https://ub.zhonguo1118.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：https://et.zhonguo4118.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：https://aa.zhonguo3118.cn

[B07] while 循环
来源：https://uh.zhonguo7118.cn

Py:   while i < 10: i += 1
来源：https://om.zhonguo1118.cn

PHP:  while ($i < 10) { $i++; }
来源：https://wj.zhonguo5118.cn

JS:   while (i < 10) { i++; }
来源：https://up.zhonguo8118.cn

TS:   while (i < 10) { i++; }
来源：https://do.zhonguo6118.cn

Java: while (i < 10) { i++; }
来源：https://cr.zhonguo7118.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：https://vj.zhonguo2118.cn

Ruby: while i < 10; i += 1; end
来源：https://cu.zhonguo2118.cn

C#:   while (i < 10) { i++; }
来源：https://np.zhonguo4118.cn

[B08] do-while（至少执行一次）
来源：https://mw.zhonguo8118.cn

Py:   # 无 do-while：用 while True + break
来源：https://tp.zhonguo5118.cn

PHP:  do { $i++; } while ($i < 10);
来源：https://as.zhonguo1118.cn

JS:   do { i++; } while (i < 10);
来源：https://py.zhonguo4118.cn

TS:   do { i++; } while (i < 10);
来源：https://no.zhonguo4118.cn

Java: do { i++; } while (i < 10);
来源：https://sx.zhonguo8118.cn

Go:   for { i++; if i >= 10 { break } }
来源：https://ep.zhonguo7118.cn

Ruby: begin; i += 1; end while i < 10
来源：https://nq.zhonguo7118.cn

C#:   do { i++; } while (i < 10);
来源：https://qa.zhonguo5118.cn

[B09] break 与 continue
来源：https://te.zhonguo5118.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：https://vu.zhonguo1118.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：https://ra.zhonguo6118.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://uy.zhonguo4118.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://dj.zhonguo4118.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://nj.zhonguo7118.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：https://wu.zhonguo8118.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：https://nn.zhonguo8118.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://wt.zhonguo1118.cn

[B10] 遍历同时拿索引
来源：https://pz.zhonguo2118.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：https://gz.zhonguo7118.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：https://gk.zhonguo1118.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：https://iz.zhonguo4118.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：https://ac.zhonguo2118.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：https://yb.zhonguo7118.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：https://zf.zhonguo4118.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：https://as.zhonguo4118.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：https://wc.zhonguo3118.cn

[B11] 生成数字序列 / 区间
来源：https://xt.zhonguo3118.cn

Py:   list(range(0, 10, 2))
来源：https://xo.zhonguo4118.cn


<!-- 参考信息 -->