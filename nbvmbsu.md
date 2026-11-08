代发 wailian999

Ruby: 42.to_s
来源：https://sb.zhonguo2118.cn

C#:   42.ToString()
来源：https://vn.zhonguo8118.cn

[A08] 取整与四舍五入
来源：https://we.zhonguo4118.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：https://ba.zhonguo8118.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：https://fj.zhonguo7118.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：https://vu.zhonguo5118.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：https://qo.zhonguo7118.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：https://ou.zhonguo5118.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：https://ga.zhonguo3118.cn

Ruby: 3.567.round(2); 3.9.floor
来源：https://hn.zhonguo4118.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：https://jg.zhonguo3118.cn

[A09] 绝对值与最大最小值
来源：https://qp.zhonguo5118.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：https://tr.zhonguo6118.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：https://ve.zhonguo3118.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：https://cu.zhonguo8118.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：https://pr.zhonguo3118.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：https://hi.zhonguo7118.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：https://af.zhonguo8118.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：https://af.zhonguo1118.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：https://go.zhonguo4118.cn

[A10] 生成随机数
来源：https://rq.zhonguo7118.cn

Py:   import random; random.randint(1, 100)
来源：https://dv.zhonguo4118.cn

PHP:  random_int(1, 100);
来源：https://ct.zhonguo5118.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：https://ze.zhonguo8118.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：https://kk.zhonguo4118.cn

Java: new Random().nextInt(100) + 1
来源：https://ve.zhonguo8118.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：https://hz.zhonguo7118.cn

Ruby: rand(1..100)
来源：https://cg.zhonguo4118.cn

C#:   new Random().Next(1, 101)
来源：https://kd.zhonguo4118.cn

[A11] 条件表达式（三元）
来源：https://pr.zhonguo8118.cn

Py:   "yes" if x > 0 else "no"
来源：https://ic.zhonguo2118.cn

PHP:  $x > 0 ? "yes" : "no"
来源：https://ae.zhonguo7118.cn

JS:   x > 0 ? "yes" : "no"
来源：https://oo.zhonguo6118.cn

TS:   x > 0 ? "yes" : "no"
来源：https://tj.zhonguo5118.cn

Java: x > 0 ? "yes" : "no"
来源：https://rd.zhonguo1118.cn

Go:   // 无三元运算符，需用 if 语句
来源：https://rp.zhonguo5118.cn

Ruby: x > 0 ? "yes" : "no"
来源：https://yx.zhonguo8118.cn

C#:   x > 0 ? "yes" : "no"
来源：https://al.zhonguo2118.cn

[A12] 字符串插值 / 格式化
来源：https://gb.zhonguo5118.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：https://fy.zhonguo3118.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：https://sa.zhonguo4118.cn

JS:   `Hello, ${name}!`
来源：https://ig.zhonguo3118.cn

TS:   `Hello, ${name}!`
来源：https://as.zhonguo3118.cn

Java: "Hello, %s!".formatted(name)
来源：https://uv.zhonguo3118.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：https://hn.zhonguo2118.cn

Ruby: "Hello, #{name}!"
来源：https://bz.zhonguo7118.cn

C#:   $"Hello, {name}!"
来源：https://kh.zhonguo3118.cn

[A13] 多行字符串（练习 \n 转义）
来源：https://kf.zhonguo3118.cn

Py:   "第一行\n第二行"
来源：https://fd.zhonguo7118.cn

PHP:  "第一行\n第二行"
来源：https://co.zhonguo5118.cn

JS:   "第一行\n第二行"
来源：https://ra.zhonguo7118.cn

TS:   "第一行\n第二行"
来源：https://nd.zhonguo8118.cn

Java: "第一行\n第二行"
来源：https://ki.zhonguo5118.cn

Go:   "第一行\n第二行"
来源：https://fn.zhonguo2118.cn

Ruby: "第一行\n第二行"
来源：https://we.zhonguo5118.cn

C#:   "第一行\n第二行"
来源：https://dd.zhonguo4118.cn

[A14] 注释写法
来源：https://zz.zhonguo2118.cn

Py:   # 单行；三引号字符串可作多行说明
来源：https://ds.zhonguo1118.cn

PHP:  // 或 # 单行；/* 多行 */
来源：https://qz.zhonguo5118.cn

JS:   // 单行；/* 多行 */
来源：https://lr.zhonguo1118.cn

TS:   // 单行；/* 多行 */
来源：https://aa.zhonguo4118.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：https://tj.zhonguo6118.cn

Go:   // 单行；/* 多行 */
来源：https://yi.zhonguo3118.cn

Ruby: # 单行；=begin 多行 =end
来源：https://rj.zhonguo3118.cn

C#:   // 单行；/* 多行 */
来源：https://tv.zhonguo2118.cn

[A15] 空值判断与默认值
来源：https://uc.zhonguo1118.cn

Py:   value = data or "默认值"
来源：https://dv.zhonguo1118.cn

PHP:  $value = $data ?? "默认值";
来源：https://hy.zhonguo6118.cn

JS:   const value = data ?? "默认值";
来源：https://bp.zhonguo6118.cn

TS:   const value = data ?? "默认值";
来源：https://zp.zhonguo3118.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：https://pf.zhonguo3118.cn

Go:   if data == "" { data = "默认值" }
来源：https://gc.zhonguo6118.cn

Ruby: value = data || "默认值"
来源：https://kq.zhonguo2118.cn

C#:   var value = data ?? "默认值";
来源：https://tw.zhonguo2118.cn

[A16] 真假值判断规则
来源：https://ap.zhonguo2118.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：https://de.zhonguo7118.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：https://wk.zhonguo1118.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：https://va.zhonguo2118.cn

TS:   if (!x) {}
来源：https://sw.zhonguo5118.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：https://tx.zhonguo2118.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：https://rm.zhonguo7118.cn

Ruby: unless x            # nil 与 false 为假
来源：https://gh.zhonguo5118.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：https://fo.zhonguo4118.cn

[A17] 位运算
来源：https://va.zhonguo5118.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://kb.zhonguo4118.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：https://da.zhonguo8118.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://bc.zhonguo4118.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：https://iz.zhonguo3118.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://br.zhonguo8118.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：https://im.zhonguo1118.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://ur.zhonguo5118.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://sy.zhonguo7118.cn

[A18] 字符与 ASCII 码互转
来源：https://pe.zhonguo4118.cn

Py:   ord("A"); chr(65)
来源：https://yj.zhonguo3118.cn

PHP:  ord("A"); chr(65)
来源：https://wc.zhonguo4118.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：https://qw.zhonguo2118.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：https://xb.zhonguo7118.cn

Java: (int) 'A'; (char) 65
来源：https://fb.zhonguo3118.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：https://wj.zhonguo3118.cn

Ruby: "A".ord; 65.chr
来源：https://qm.zhonguo6118.cn

C#:   (int)'A'; (char)65
来源：https://fb.zhonguo6118.cn

[A19] 交换两个变量
来源：https://tm.zhonguo7118.cn

Py:   a, b = b, a
来源：https://it.zhonguo2118.cn

PHP:  [$a, $b] = [$b, $a];
来源：https://pz.zhonguo3118.cn

JS:   [a, b] = [b, a];
来源：https://ou.zhonguo3118.cn

TS:   [a, b] = [b, a];
来源：https://ud.zhonguo5118.cn

Java: int t = a; a = b; b = t;
来源：https://hr.zhonguo3118.cn

Go:   a, b = b, a
来源：https://zd.zhonguo4118.cn

Ruby: a, b = b, a
来源：https://wb.zhonguo3118.cn

C#:   (a, b) = (b, a);
来源：https://ts.zhonguo6118.cn

[A20] 读取标准输入
来源：https://de.zhonguo2118.cn

Py:   name = input("请输入：")
来源：https://pt.zhonguo7118.cn

PHP:  $name = trim(fgets(STDIN));
来源：https://uq.zhonguo1118.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：https://jq.zhonguo1118.cn

TS:   // Node.js：readline 模块
来源：https://my.zhonguo8118.cn

Java: new Scanner(System.in).nextLine()
来源：https://nr.zhonguo6118.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：https://vw.zhonguo4118.cn

Ruby: gets.chomp
来源：https://jk.zhonguo1118.cn

C#:   Console.ReadLine();
来源：https://dd.zhonguo3118.cn

[A21] 保留指定小数位输出
来源：https://rl.zhonguo6118.cn

Py:   f"{3.14159:.2f}"
来源：https://ip.zhonguo8118.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：https://kq.zhonguo7118.cn

JS:   (3.14159).toFixed(2)
来源：https://mg.zhonguo8118.cn

TS:   (3.14159).toFixed(2)
来源：https://ms.zhonguo5118.cn

Java: String.format("%.2f", 3.14159)
来源：https://iz.zhonguo1118.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：https://gv.zhonguo4118.cn

Ruby: format("%.2f", 3.14159)
来源：https://ro.zhonguo5118.cn

C#:   3.14159.ToString("F2")
来源：https://cp.zhonguo2118.cn

[A22] 获取字符串长度
来源：https://oe.zhonguo6118.cn

Py:   len(s)
来源：https://ra.zhonguo1118.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：https://zp.zhonguo4118.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：https://qa.zhonguo3118.cn

TS:   s.length
来源：https://dk.zhonguo1118.cn

Java: s.length()
来源：https://kk.zhonguo6118.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：https://mt.zhonguo8118.cn

Ruby: s.length
来源：https://fy.zhonguo6118.cn

C#:   s.Length
来源：https://qu.zhonguo5118.cn

[A23] 大小写转换
来源：https://id.zhonguo5118.cn

Py:   s.upper(); s.lower(); s.title()
来源：https://kd.zhonguo5118.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：https://ag.zhonguo4118.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：https://jp.zhonguo7118.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：https://xq.zhonguo4118.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：https://lm.zhonguo7118.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：https://hc.zhonguo8118.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：https://sm.zhonguo5118.cn

C#:   s.ToUpper(); s.ToLower()
来源：https://ft.zhonguo7118.cn

[A24] 去除首尾空白
来源：https://ht.zhonguo1118.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：https://lt.zhonguo1118.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：https://rf.zhonguo5118.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://rx.zhonguo3118.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://nw.zhonguo8118.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：https://hq.zhonguo3118.cn

Go:   strings.TrimSpace(s)
来源：https://oa.zhonguo1118.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：https://ix.zhonguo1118.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：https://jk.zhonguo2118.cn

[A25] 字符串比较
来源：https://lf.zhonguo4118.cn

Py:   s1 == s2; s1 != s2
来源：https://ib.zhonguo8118.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：https://je.zhonguo2118.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：https://rw.zhonguo6118.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：https://qa.zhonguo4118.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：https://xx.zhonguo7118.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：https://gl.zhonguo1118.cn

Ruby: s1 == s2; s1 <=> s2
来源：https://wj.zhonguo5118.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：https://lf.zhonguo5118.cn

[A26] 类型转换总览
来源：https://ni.zhonguo5118.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：https://xq.zhonguo7118.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：https://dp.zhonguo4118.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：https://zh.zhonguo4118.cn

TS:   Number() String() Boolean() x as number
来源：https://yv.zhonguo6118.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：https://fq.zhonguo5118.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：https://mn.zhonguo6118.cn

Ruby: to_i to_f to_s to_sym to_a
来源：https://lk.zhonguo7118.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：https://hm.zhonguo6118.cn

================================================================================
来源：https://nm.zhonguo2118.cn

B. 流程控制
来源：https://nn.zhonguo6118.cn

================================================================================
来源：https://yc.zhonguo2118.cn

[B01] 条件判断 if / else
来源：https://nq.zhonguo8118.cn

Py:   result = "正" if x > 0 else "非正"
来源：https://vo.zhonguo5118.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：https://ii.zhonguo1118.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：https://gp.zhonguo2118.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：https://xq.zhonguo4118.cn

Java: String r = x > 0 ? "正" : "非正";
来源：https://tc.zhonguo5118.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：https://sc.zhonguo4118.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：https://qv.zhonguo4118.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：https://eb.zhonguo2118.cn

[B02] 多分支 else if / elif
来源：https://xs.zhonguo7118.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：https://yw.zhonguo7118.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：https://ct.zhonguo4118.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://qt.zhonguo3118.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://bn.zhonguo1118.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://hi.zhonguo2118.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：https://og.zhonguo8118.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：https://gk.zhonguo3118.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://bb.zhonguo6118.cn

[B03] switch / match / case
来源：https://be.zhonguo3118.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：https://vc.zhonguo4118.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：https://bc.zhonguo2118.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://ym.zhonguo1118.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://rs.zhonguo4118.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：https://ng.zhonguo3118.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：https://jh.zhonguo8118.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：https://vp.zhonguo8118.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：https://pg.zhonguo1118.cn

[B04] for 计数循环
来源：https://mt.zhonguo1118.cn

Py:   for i in range(10): print(i)
来源：https://wt.zhonguo3118.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：https://ie.zhonguo5118.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://kr.zhonguo4118.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://ur.zhonguo3118.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：https://vs.zhonguo7118.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：https://in.zhonguo2118.cn

Ruby: 10.times { |i| puts i }
来源：https://dt.zhonguo5118.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：https://jx.zhonguo5118.cn

[B05] 遍历数组 / 列表
来源：https://rj.zhonguo2118.cn

Py:   for item in arr: print(item)
来源：https://mv.zhonguo6118.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：https://ti.zhonguo4118.cn

JS:   for (const item of arr) { console.log(item); }
来源：https://ht.zhonguo7118.cn

TS:   for (const item of arr) { console.log(item); }
来源：https://sz.zhonguo4118.cn

Java: for (var item : arr) { System.out.println(item); }
来源：https://pb.zhonguo6118.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：https://mh.zhonguo4118.cn

Ruby: arr.each { |item| puts item }
来源：https://nx.zhonguo1118.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：https://wt.zhonguo5118.cn

[B06] 遍历字典 / 对象
来源：https://xr.zhonguo2118.cn

Py:   for k, v in d.items(): print(k, v)
来源：https://qd.zhonguo4118.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：https://gs.zhonguo7118.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://ki.zhonguo6118.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://bh.zhonguo7118.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：https://iz.zhonguo7118.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：https://hc.zhonguo3118.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：https://zd.zhonguo8118.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：https://ui.zhonguo1118.cn

[B07] while 循环
来源：https://uj.zhonguo1118.cn

Py:   while i < 10: i += 1
来源：https://bz.zhonguo7118.cn

PHP:  while ($i < 10) { $i++; }
来源：https://dc.zhonguo3118.cn

JS:   while (i < 10) { i++; }
来源：https://az.zhonguo5118.cn

TS:   while (i < 10) { i++; }
来源：https://uh.zhonguo6118.cn

Java: while (i < 10) { i++; }
来源：https://tw.zhonguo7118.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：https://hx.zhonguo2118.cn

Ruby: while i < 10; i += 1; end
来源：https://vl.zhonguo2118.cn

C#:   while (i < 10) { i++; }
来源：https://ka.zhonguo8118.cn

[B08] do-while（至少执行一次）
来源：https://do.zhonguo7118.cn

Py:   # 无 do-while：用 while True + break
来源：https://go.zhonguo5118.cn

PHP:  do { $i++; } while ($i < 10);
来源：https://ll.zhonguo8118.cn

JS:   do { i++; } while (i < 10);
来源：https://mc.zhonguo4118.cn

TS:   do { i++; } while (i < 10);
来源：https://ij.zhonguo5118.cn

Java: do { i++; } while (i < 10);
来源：https://dv.zhonguo1118.cn

Go:   for { i++; if i >= 10 { break } }
来源：https://ri.zhonguo4118.cn

Ruby: begin; i += 1; end while i < 10
来源：https://wa.zhonguo6118.cn

C#:   do { i++; } while (i < 10);
来源：https://qx.zhonguo2118.cn

[B09] break 与 continue
来源：https://fz.zhonguo5118.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：https://vd.zhonguo3118.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：https://zw.zhonguo6118.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://nk.zhonguo8118.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://if.zhonguo7118.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://ar.zhonguo4118.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：https://cv.zhonguo5118.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：https://gg.zhonguo4118.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://aa.zhonguo3118.cn

[B10] 遍历同时拿索引
来源：https://nq.zhonguo6118.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：https://qh.zhonguo3118.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：https://xx.zhonguo5118.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：https://nf.zhonguo6118.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：https://of.zhonguo5118.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：https://io.zhonguo3118.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：https://ga.zhonguo6118.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：https://nq.zhonguo7118.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：https://cv.zhonguo3118.cn

[B11] 生成数字序列 / 区间
来源：https://wa.zhonguo2118.cn

Py:   list(range(0, 10, 2))
来源：https://zs.zhonguo3118.cn

PHP:  range(0, 10, 2);
来源：https://mp.zhonguo4118.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：https://jr.zhonguo6118.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：https://bf.zhonguo2118.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：https://ci.zhonguo4118.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：https://vw.zhonguo6118.cn

Ruby: (0...10).step(2).to_a
来源：https://hd.zhonguo7118.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：https://bi.zhonguo5118.cn

[B12] 跳出多层循环
来源：https://fs.zhonguo4118.cn

Py:   # 无标签跳转：抽成函数用 return
来源：https://tl.zhonguo4118.cn

PHP:  # 无标签：用 goto 或函数返回
来源：https://jm.zhonguo3118.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：https://tm.zhonguo8118.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：https://om.zhonguo4118.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：https://gc.zhonguo3118.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：https://xq.zhonguo7118.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：https://qy.zhonguo7118.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：https://ry.zhonguo7118.cn

[B13] 判断是否为数字
来源：https://kt.zhonguo8118.cn

Py:   isinstance(x, (int, float))
来源：https://pl.zhonguo6118.cn

PHP:  is_numeric($x)
来源：https://cm.zhonguo2118.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：https://wx.zhonguo8118.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：https://qz.zhonguo5118.cn

Java: x instanceof Number
来源：https://od.zhonguo4118.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：https://km.zhonguo8118.cn

Ruby: x.is_a?(Numeric)
来源：https://ys.zhonguo1118.cn

C#:   x is int or double or decimal
来源：https://yq.zhonguo7118.cn

[B14] 判断值是否在集合内
来源：https://au.zhonguo7118.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：https://hi.zhonguo8118.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：https://ka.zhonguo3118.cn

JS:   [1, 2, 3].includes(x)
来源：https://xo.zhonguo4118.cn

TS:   [1, 2, 3].includes(x)
来源：https://tg.zhonguo8118.cn

Java: List.of(1, 2, 3).contains(x)
来源：https://hm.zhonguo4118.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：https://qh.zhonguo1118.cn


<!-- 参考信息 -->