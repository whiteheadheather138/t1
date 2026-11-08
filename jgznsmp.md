代发 wailian999

Ruby: 42.to_s
来源：https://ry.zhonguo8118.cn

C#:   42.ToString()
来源：https://eo.zhonguo1118.cn

[A08] 取整与四舍五入
来源：https://nk.zhonguo7118.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：https://ow.zhonguo6118.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：https://tz.zhonguo3118.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：https://fg.zhonguo2118.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：https://bp.zhonguo4118.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：https://ij.zhonguo3118.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：https://eq.zhonguo8118.cn

Ruby: 3.567.round(2); 3.9.floor
来源：https://wc.zhonguo5118.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：https://yt.zhonguo8118.cn

[A09] 绝对值与最大最小值
来源：https://eg.zhonguo2118.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：https://wk.zhonguo6118.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：https://op.zhonguo2118.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：https://vo.zhonguo6118.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：https://mo.zhonguo5118.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：https://lf.zhonguo4118.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：https://fz.zhonguo5118.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：https://zl.zhonguo4118.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：https://sc.zhonguo4118.cn

[A10] 生成随机数
来源：https://de.zhonguo3118.cn

Py:   import random; random.randint(1, 100)
来源：https://vx.zhonguo6118.cn

PHP:  random_int(1, 100);
来源：https://zm.zhonguo6118.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：https://pa.zhonguo3118.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：https://vc.zhonguo3118.cn

Java: new Random().nextInt(100) + 1
来源：https://ha.zhonguo1118.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：https://or.zhonguo6118.cn

Ruby: rand(1..100)
来源：https://ej.zhonguo1118.cn

C#:   new Random().Next(1, 101)
来源：https://kf.zhonguo8118.cn

[A11] 条件表达式（三元）
来源：https://tu.zhonguo1118.cn

Py:   "yes" if x > 0 else "no"
来源：https://sx.zhonguo6118.cn

PHP:  $x > 0 ? "yes" : "no"
来源：https://nk.zhonguo8118.cn

JS:   x > 0 ? "yes" : "no"
来源：https://md.zhonguo5118.cn

TS:   x > 0 ? "yes" : "no"
来源：https://ib.zhonguo4118.cn

Java: x > 0 ? "yes" : "no"
来源：https://cp.zhonguo5118.cn

Go:   // 无三元运算符，需用 if 语句
来源：https://by.zhonguo5118.cn

Ruby: x > 0 ? "yes" : "no"
来源：https://va.zhonguo3118.cn

C#:   x > 0 ? "yes" : "no"
来源：https://qh.zhonguo3118.cn

[A12] 字符串插值 / 格式化
来源：https://zx.zhonguo4118.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：https://zw.zhonguo2118.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：https://yg.zhonguo8118.cn

JS:   `Hello, ${name}!`
来源：https://so.zhonguo1118.cn

TS:   `Hello, ${name}!`
来源：https://xe.zhonguo5118.cn

Java: "Hello, %s!".formatted(name)
来源：https://do.zhonguo7118.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：https://nm.zhonguo4118.cn

Ruby: "Hello, #{name}!"
来源：https://mo.zhonguo4118.cn

C#:   $"Hello, {name}!"
来源：https://rw.zhonguo2118.cn

[A13] 多行字符串（练习 \n 转义）
来源：https://lt.zhonguo8118.cn

Py:   "第一行\n第二行"
来源：https://sy.zhonguo1118.cn

PHP:  "第一行\n第二行"
来源：https://xf.zhonguo1118.cn

JS:   "第一行\n第二行"
来源：https://me.zhonguo4118.cn

TS:   "第一行\n第二行"
来源：https://ez.zhonguo7118.cn

Java: "第一行\n第二行"
来源：https://ak.zhonguo1118.cn

Go:   "第一行\n第二行"
来源：https://ps.zhonguo5118.cn

Ruby: "第一行\n第二行"
来源：https://fq.zhonguo3118.cn

C#:   "第一行\n第二行"
来源：https://fv.zhonguo6118.cn

[A14] 注释写法
来源：https://ws.zhonguo2118.cn

Py:   # 单行；三引号字符串可作多行说明
来源：https://nz.zhonguo1118.cn

PHP:  // 或 # 单行；/* 多行 */
来源：https://fm.zhonguo8118.cn

JS:   // 单行；/* 多行 */
来源：https://fn.zhonguo5118.cn

TS:   // 单行；/* 多行 */
来源：https://bj.zhonguo7118.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：https://tu.zhonguo8118.cn

Go:   // 单行；/* 多行 */
来源：https://ow.zhonguo8118.cn

Ruby: # 单行；=begin 多行 =end
来源：https://xg.zhonguo2118.cn

C#:   // 单行；/* 多行 */
来源：https://le.zhonguo4118.cn

[A15] 空值判断与默认值
来源：https://wq.zhonguo3118.cn

Py:   value = data or "默认值"
来源：https://bz.zhonguo7118.cn

PHP:  $value = $data ?? "默认值";
来源：https://cu.zhonguo7118.cn

JS:   const value = data ?? "默认值";
来源：https://py.zhonguo4118.cn

TS:   const value = data ?? "默认值";
来源：https://mv.zhonguo2118.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：https://qt.zhonguo5118.cn

Go:   if data == "" { data = "默认值" }
来源：https://xf.zhonguo6118.cn

Ruby: value = data || "默认值"
来源：https://ge.zhonguo6118.cn

C#:   var value = data ?? "默认值";
来源：https://mc.zhonguo1118.cn

[A16] 真假值判断规则
来源：https://qz.zhonguo2118.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：https://io.zhonguo3118.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：https://pc.zhonguo8118.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：https://nk.zhonguo7118.cn

TS:   if (!x) {}
来源：https://so.zhonguo3118.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：https://yf.zhonguo8118.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：https://dx.zhonguo2118.cn

Ruby: unless x            # nil 与 false 为假
来源：https://hy.zhonguo1118.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：https://lo.zhonguo2118.cn

[A17] 位运算
来源：https://hm.zhonguo4118.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://re.zhonguo1118.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：https://gk.zhonguo1118.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://sl.zhonguo2118.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：https://jk.zhonguo4118.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://zn.zhonguo8118.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：https://pd.zhonguo7118.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://yw.zhonguo8118.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://nu.zhonguo5118.cn

[A18] 字符与 ASCII 码互转
来源：https://no.zhonguo6118.cn

Py:   ord("A"); chr(65)
来源：https://us.zhonguo6118.cn

PHP:  ord("A"); chr(65)
来源：https://xc.zhonguo8118.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：https://bk.zhonguo3118.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：https://ws.zhonguo2118.cn

Java: (int) 'A'; (char) 65
来源：https://vd.zhonguo5118.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：https://uw.zhonguo5118.cn

Ruby: "A".ord; 65.chr
来源：https://og.zhonguo1118.cn

C#:   (int)'A'; (char)65
来源：https://os.zhonguo1118.cn

[A19] 交换两个变量
来源：https://cz.zhonguo7118.cn

Py:   a, b = b, a
来源：https://pg.zhonguo8118.cn

PHP:  [$a, $b] = [$b, $a];
来源：https://bp.zhonguo6118.cn

JS:   [a, b] = [b, a];
来源：https://mg.zhonguo8118.cn

TS:   [a, b] = [b, a];
来源：https://bl.zhonguo6118.cn

Java: int t = a; a = b; b = t;
来源：https://wi.zhonguo1118.cn

Go:   a, b = b, a
来源：https://af.zhonguo3118.cn

Ruby: a, b = b, a
来源：https://st.zhonguo2118.cn

C#:   (a, b) = (b, a);
来源：https://sf.zhonguo8118.cn

[A20] 读取标准输入
来源：https://hz.zhonguo8118.cn

Py:   name = input("请输入：")
来源：https://ky.zhonguo4118.cn

PHP:  $name = trim(fgets(STDIN));
来源：https://ep.zhonguo2118.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：https://fa.zhonguo1118.cn

TS:   // Node.js：readline 模块
来源：https://my.zhonguo1118.cn

Java: new Scanner(System.in).nextLine()
来源：https://qd.zhonguo1118.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：https://mw.zhonguo5118.cn

Ruby: gets.chomp
来源：https://hk.zhonguo5118.cn

C#:   Console.ReadLine();
来源：https://cg.zhonguo2118.cn

[A21] 保留指定小数位输出
来源：https://ly.zhonguo5118.cn

Py:   f"{3.14159:.2f}"
来源：https://zr.zhonguo1118.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：https://mp.zhonguo4118.cn

JS:   (3.14159).toFixed(2)
来源：https://zz.zhonguo2118.cn

TS:   (3.14159).toFixed(2)
来源：https://fm.zhonguo3118.cn

Java: String.format("%.2f", 3.14159)
来源：https://of.zhonguo5118.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：https://tx.zhonguo8118.cn

Ruby: format("%.2f", 3.14159)
来源：https://bm.zhonguo5118.cn

C#:   3.14159.ToString("F2")
来源：https://da.zhonguo7118.cn

[A22] 获取字符串长度
来源：https://ix.zhonguo4118.cn

Py:   len(s)
来源：https://pa.zhonguo2118.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：https://hh.zhonguo7118.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：https://wv.zhonguo1118.cn

TS:   s.length
来源：https://kr.zhonguo5118.cn

Java: s.length()
来源：https://hs.zhonguo6118.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：https://ss.zhonguo1118.cn

Ruby: s.length
来源：https://dh.zhonguo1118.cn

C#:   s.Length
来源：https://xp.zhonguo8118.cn

[A23] 大小写转换
来源：https://pl.zhonguo6118.cn

Py:   s.upper(); s.lower(); s.title()
来源：https://qi.zhonguo7118.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：https://sv.zhonguo4118.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：https://ii.zhonguo8118.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：https://ta.zhonguo3118.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：https://hg.zhonguo3118.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：https://ai.zhonguo1118.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：https://kw.zhonguo4118.cn

C#:   s.ToUpper(); s.ToLower()
来源：https://ie.zhonguo2118.cn

[A24] 去除首尾空白
来源：https://xy.zhonguo5118.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：https://mo.zhonguo7118.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：https://zy.zhonguo7118.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://ut.zhonguo6118.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://zv.zhonguo5118.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：https://yk.zhonguo4118.cn

Go:   strings.TrimSpace(s)
来源：https://dq.zhonguo8118.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：https://hx.zhonguo6118.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：https://he.zhonguo8118.cn

[A25] 字符串比较
来源：https://qd.zhonguo1118.cn

Py:   s1 == s2; s1 != s2
来源：https://ny.zhonguo1118.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：https://zc.zhonguo2118.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：https://nn.zhonguo5118.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：https://nu.zhonguo5118.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：https://qr.zhonguo6118.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：https://dl.zhonguo7118.cn

Ruby: s1 == s2; s1 <=> s2
来源：https://iw.zhonguo4118.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：https://ea.zhonguo2118.cn

[A26] 类型转换总览
来源：https://mw.zhonguo5118.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：https://ri.zhonguo4118.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：https://db.zhonguo2118.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：https://xi.zhonguo3118.cn

TS:   Number() String() Boolean() x as number
来源：https://lo.zhonguo7118.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：https://du.zhonguo7118.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：https://do.zhonguo2118.cn

Ruby: to_i to_f to_s to_sym to_a
来源：https://pj.zhonguo5118.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：https://qo.zhonguo3118.cn

================================================================================
来源：https://sv.zhonguo6118.cn

B. 流程控制
来源：https://nk.zhonguo1118.cn

================================================================================
来源：https://mw.zhonguo8118.cn

[B01] 条件判断 if / else
来源：https://xe.zhonguo1118.cn

Py:   result = "正" if x > 0 else "非正"
来源：https://ma.zhonguo2118.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：https://nm.zhonguo1118.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：https://uo.zhonguo3118.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：https://zg.zhonguo7118.cn

Java: String r = x > 0 ? "正" : "非正";
来源：https://lw.zhonguo2118.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：https://fg.zhonguo8118.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：https://ad.zhonguo1118.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：https://an.zhonguo5118.cn

[B02] 多分支 else if / elif
来源：https://dv.zhonguo7118.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：https://jm.zhonguo6118.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：https://lr.zhonguo8118.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://km.zhonguo1118.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://gt.zhonguo2118.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://qa.zhonguo2118.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：https://nb.zhonguo7118.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：https://lp.zhonguo5118.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://me.zhonguo8118.cn

[B03] switch / match / case
来源：https://hd.zhonguo7118.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：https://lt.zhonguo8118.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：https://pl.zhonguo3118.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://gv.zhonguo5118.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://jr.zhonguo8118.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：https://bm.zhonguo3118.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：https://pm.zhonguo6118.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：https://mp.zhonguo8118.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：https://xt.zhonguo8118.cn

[B04] for 计数循环
来源：https://ml.zhonguo8118.cn

Py:   for i in range(10): print(i)
来源：https://it.zhonguo2118.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：https://ea.zhonguo2118.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://pn.zhonguo4118.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://ii.zhonguo8118.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：https://rx.zhonguo2118.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：https://os.zhonguo2118.cn

Ruby: 10.times { |i| puts i }
来源：https://dz.zhonguo5118.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：https://pw.zhonguo3118.cn

[B05] 遍历数组 / 列表
来源：https://lg.zhonguo3118.cn

Py:   for item in arr: print(item)
来源：https://zd.zhonguo3118.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：https://ul.zhonguo4118.cn

JS:   for (const item of arr) { console.log(item); }
来源：https://wt.zhonguo6118.cn

TS:   for (const item of arr) { console.log(item); }
来源：https://ok.zhonguo8118.cn

Java: for (var item : arr) { System.out.println(item); }
来源：https://ud.zhonguo4118.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：https://ui.zhonguo5118.cn

Ruby: arr.each { |item| puts item }
来源：https://yv.zhonguo7118.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：https://mr.zhonguo5118.cn

[B06] 遍历字典 / 对象
来源：https://hi.zhonguo5118.cn

Py:   for k, v in d.items(): print(k, v)
来源：https://hd.zhonguo7118.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：https://kr.zhonguo2118.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://tq.zhonguo4118.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://tm.zhonguo5118.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：https://tx.zhonguo4118.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：https://up.zhonguo5118.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：https://kr.zhonguo2118.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：https://mv.zhonguo6118.cn

[B07] while 循环
来源：https://yo.zhonguo1118.cn

Py:   while i < 10: i += 1
来源：https://sc.zhonguo1118.cn

PHP:  while ($i < 10) { $i++; }
来源：https://ct.zhonguo6118.cn

JS:   while (i < 10) { i++; }
来源：https://bo.zhonguo7118.cn

TS:   while (i < 10) { i++; }
来源：https://sg.zhonguo5118.cn

Java: while (i < 10) { i++; }
来源：https://ft.zhonguo1118.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：https://xa.zhonguo7118.cn

Ruby: while i < 10; i += 1; end
来源：https://cr.zhonguo5118.cn

C#:   while (i < 10) { i++; }
来源：https://mm.zhonguo6118.cn

[B08] do-while（至少执行一次）
来源：https://bh.zhonguo5118.cn

Py:   # 无 do-while：用 while True + break
来源：https://nx.zhonguo2118.cn

PHP:  do { $i++; } while ($i < 10);
来源：https://wq.zhonguo7118.cn

JS:   do { i++; } while (i < 10);
来源：https://yx.zhonguo1118.cn

TS:   do { i++; } while (i < 10);
来源：https://wa.zhonguo3118.cn

Java: do { i++; } while (i < 10);
来源：https://oo.zhonguo6118.cn

Go:   for { i++; if i >= 10 { break } }
来源：https://xk.zhonguo6118.cn

Ruby: begin; i += 1; end while i < 10
来源：https://nc.zhonguo8118.cn

C#:   do { i++; } while (i < 10);
来源：https://zz.zhonguo3118.cn

[B09] break 与 continue
来源：https://tf.zhonguo8118.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：https://bd.zhonguo6118.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：https://ij.zhonguo5118.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://fn.zhonguo6118.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://zb.zhonguo2118.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://ox.zhonguo8118.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：https://yh.zhonguo7118.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：https://hh.zhonguo8118.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://fk.zhonguo4118.cn

[B10] 遍历同时拿索引
来源：https://lw.zhonguo8118.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：https://oz.zhonguo7118.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：https://ep.zhonguo7118.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：https://cb.zhonguo1118.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：https://xh.zhonguo7118.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：https://fo.zhonguo8118.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：https://db.zhonguo3118.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：https://yn.zhonguo7118.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：https://qv.zhonguo1118.cn

[B11] 生成数字序列 / 区间
来源：https://rt.zhonguo5118.cn

Py:   list(range(0, 10, 2))
来源：https://gz.zhonguo1118.cn

PHP:  range(0, 10, 2);
来源：https://dl.zhonguo3118.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：https://db.zhonguo1118.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：https://yv.zhonguo5118.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：https://ol.zhonguo5118.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：https://gx.zhonguo4118.cn

Ruby: (0...10).step(2).to_a
来源：https://hu.zhonguo8118.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：https://zm.zhonguo1118.cn

[B12] 跳出多层循环
来源：https://xc.zhonguo1118.cn

Py:   # 无标签跳转：抽成函数用 return
来源：https://xm.zhonguo4118.cn

PHP:  # 无标签：用 goto 或函数返回
来源：https://vp.zhonguo7118.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：https://wb.zhonguo5118.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：https://kc.zhonguo5118.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：https://hh.zhonguo1118.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：https://ha.zhonguo6118.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：https://bf.zhonguo5118.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：https://bg.zhonguo4118.cn

[B13] 判断是否为数字
来源：https://lt.zhonguo8118.cn

Py:   isinstance(x, (int, float))
来源：https://yk.zhonguo2118.cn

PHP:  is_numeric($x)
来源：https://nk.zhonguo3118.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：https://ez.zhonguo2118.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：https://fa.zhonguo2118.cn

Java: x instanceof Number
来源：https://ij.zhonguo3118.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：https://zx.zhonguo4118.cn

Ruby: x.is_a?(Numeric)
来源：https://bk.zhonguo1118.cn

C#:   x is int or double or decimal
来源：https://ep.zhonguo5118.cn

[B14] 判断值是否在集合内
来源：https://ht.zhonguo6118.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：https://vj.zhonguo4118.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：https://qw.zhonguo2118.cn

JS:   [1, 2, 3].includes(x)
来源：https://ah.zhonguo5118.cn

TS:   [1, 2, 3].includes(x)
来源：https://gm.zhonguo6118.cn

Java: List.of(1, 2, 3).contains(x)
来源：https://th.zhonguo1118.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：https://yl.zhonguo2118.cn


<!-- 参考信息 -->