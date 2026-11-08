代发 wailian999

C#:   int.Parse("42"); double.Parse("3.14")
来源：https://nh.zhonguo1118.cn

[A07] 数字转字符串
来源：https://sm.zhonguo6118.cn

Py:   str(42)
来源：https://ci.zhonguo8118.cn

PHP:  (string) 42; strval(42)
来源：https://as.zhonguo5118.cn

JS:   String(42); (42).toString()
来源：https://bw.zhonguo1118.cn

TS:   String(42)
来源：https://ig.zhonguo4118.cn

Java: String.valueOf(42); Integer.toString(42)
来源：https://vh.zhonguo4118.cn

Go:   strconv.Itoa(42)
来源：https://sb.zhonguo1118.cn

Ruby: 42.to_s
来源：https://rs.zhonguo5118.cn

C#:   42.ToString()
来源：https://qr.zhonguo4118.cn

[A08] 取整与四舍五入
来源：https://ju.zhonguo3118.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：https://bg.zhonguo3118.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：https://ev.zhonguo7118.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：https://dr.zhonguo6118.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：https://xv.zhonguo8118.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：https://ds.zhonguo4118.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：https://nz.zhonguo3118.cn

Ruby: 3.567.round(2); 3.9.floor
来源：https://rf.zhonguo3118.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：https://jn.zhonguo8118.cn

[A09] 绝对值与最大最小值
来源：https://zs.zhonguo3118.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：https://uz.zhonguo2118.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：https://md.zhonguo6118.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：https://sl.zhonguo1118.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：https://ba.zhonguo3118.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：https://zi.zhonguo3118.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：https://wv.zhonguo1118.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：https://cz.zhonguo2118.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：https://hm.zhonguo5118.cn

[A10] 生成随机数
来源：https://dh.zhonguo1118.cn

Py:   import random; random.randint(1, 100)
来源：https://hs.zhonguo7118.cn

PHP:  random_int(1, 100);
来源：https://bu.zhonguo1118.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：https://xd.zhonguo6118.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：https://ss.zhonguo8118.cn

Java: new Random().nextInt(100) + 1
来源：https://ws.zhonguo1118.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：https://en.zhonguo6118.cn

Ruby: rand(1..100)
来源：https://ox.zhonguo3118.cn

C#:   new Random().Next(1, 101)
来源：https://el.zhonguo3118.cn

[A11] 条件表达式（三元）
来源：https://bu.zhonguo3118.cn

Py:   "yes" if x > 0 else "no"
来源：https://xs.zhonguo6118.cn

PHP:  $x > 0 ? "yes" : "no"
来源：https://xc.zhonguo2118.cn

JS:   x > 0 ? "yes" : "no"
来源：https://fa.zhonguo6118.cn

TS:   x > 0 ? "yes" : "no"
来源：https://lk.zhonguo3118.cn

Java: x > 0 ? "yes" : "no"
来源：https://qa.zhonguo5118.cn

Go:   // 无三元运算符，需用 if 语句
来源：https://ur.zhonguo3118.cn

Ruby: x > 0 ? "yes" : "no"
来源：https://qb.zhonguo3118.cn

C#:   x > 0 ? "yes" : "no"
来源：https://zt.zhonguo2118.cn

[A12] 字符串插值 / 格式化
来源：https://pk.zhonguo3118.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：https://qh.zhonguo5118.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：https://ec.zhonguo2118.cn

JS:   `Hello, ${name}!`
来源：https://eh.zhonguo6118.cn

TS:   `Hello, ${name}!`
来源：https://jp.zhonguo3118.cn

Java: "Hello, %s!".formatted(name)
来源：https://pm.zhonguo7118.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：https://uc.zhonguo6118.cn

Ruby: "Hello, #{name}!"
来源：https://le.zhonguo1118.cn

C#:   $"Hello, {name}!"
来源：https://gr.zhonguo4118.cn

[A13] 多行字符串（练习 \n 转义）
来源：https://jz.zhonguo6118.cn

Py:   "第一行\n第二行"
来源：https://jn.zhonguo7118.cn

PHP:  "第一行\n第二行"
来源：https://bf.zhonguo6118.cn

JS:   "第一行\n第二行"
来源：https://al.zhonguo8118.cn

TS:   "第一行\n第二行"
来源：https://su.zhonguo3118.cn

Java: "第一行\n第二行"
来源：https://rh.zhonguo3118.cn

Go:   "第一行\n第二行"
来源：https://hv.zhonguo6118.cn

Ruby: "第一行\n第二行"
来源：https://in.zhonguo8118.cn

C#:   "第一行\n第二行"
来源：https://ef.zhonguo8118.cn

[A14] 注释写法
来源：https://mr.zhonguo7118.cn

Py:   # 单行；三引号字符串可作多行说明
来源：https://cd.zhonguo5118.cn

PHP:  // 或 # 单行；/* 多行 */
来源：https://qs.zhonguo4118.cn

JS:   // 单行；/* 多行 */
来源：https://ah.zhonguo4118.cn

TS:   // 单行；/* 多行 */
来源：https://hz.zhonguo5118.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：https://ht.zhonguo7118.cn

Go:   // 单行；/* 多行 */
来源：https://sw.zhonguo3118.cn

Ruby: # 单行；=begin 多行 =end
来源：https://ic.zhonguo4118.cn

C#:   // 单行；/* 多行 */
来源：https://tz.zhonguo8118.cn

[A15] 空值判断与默认值
来源：https://jb.zhonguo3118.cn

Py:   value = data or "默认值"
来源：https://mh.zhonguo1118.cn

PHP:  $value = $data ?? "默认值";
来源：https://ow.zhonguo2118.cn

JS:   const value = data ?? "默认值";
来源：https://ub.zhonguo1118.cn

TS:   const value = data ?? "默认值";
来源：https://qe.zhonguo5118.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：https://sf.zhonguo1118.cn

Go:   if data == "" { data = "默认值" }
来源：https://ei.zhonguo1118.cn

Ruby: value = data || "默认值"
来源：https://pl.zhonguo5118.cn

C#:   var value = data ?? "默认值";
来源：https://rw.zhonguo2118.cn

[A16] 真假值判断规则
来源：https://vl.zhonguo4118.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：https://ns.zhonguo2118.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：https://eq.zhonguo8118.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：https://pc.zhonguo4118.cn

TS:   if (!x) {}
来源：https://ma.zhonguo2118.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：https://sy.zhonguo3118.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：https://fy.zhonguo5118.cn

Ruby: unless x            # nil 与 false 为假
来源：https://sl.zhonguo2118.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：https://hm.zhonguo8118.cn

[A17] 位运算
来源：https://lq.zhonguo6118.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://ar.zhonguo6118.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：https://to.zhonguo2118.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://fh.zhonguo3118.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：https://la.zhonguo6118.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://ux.zhonguo2118.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：https://fy.zhonguo2118.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://au.zhonguo7118.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://ch.zhonguo6118.cn

[A18] 字符与 ASCII 码互转
来源：https://pu.zhonguo2118.cn

Py:   ord("A"); chr(65)
来源：https://om.zhonguo4118.cn

PHP:  ord("A"); chr(65)
来源：https://um.zhonguo7118.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：https://av.zhonguo1118.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：https://gb.zhonguo5118.cn

Java: (int) 'A'; (char) 65
来源：https://fa.zhonguo1118.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：https://oc.zhonguo5118.cn

Ruby: "A".ord; 65.chr
来源：https://fl.zhonguo2118.cn

C#:   (int)'A'; (char)65
来源：https://ma.zhonguo5118.cn

[A19] 交换两个变量
来源：https://of.zhonguo5118.cn

Py:   a, b = b, a
来源：https://uk.zhonguo6118.cn

PHP:  [$a, $b] = [$b, $a];
来源：https://eo.zhonguo2118.cn

JS:   [a, b] = [b, a];
来源：https://dp.zhonguo5118.cn

TS:   [a, b] = [b, a];
来源：https://ul.zhonguo4118.cn

Java: int t = a; a = b; b = t;
来源：https://rg.zhonguo1118.cn

Go:   a, b = b, a
来源：https://tp.zhonguo1118.cn

Ruby: a, b = b, a
来源：https://dr.zhonguo5118.cn

C#:   (a, b) = (b, a);
来源：https://zz.zhonguo4118.cn

[A20] 读取标准输入
来源：https://ld.zhonguo8118.cn

Py:   name = input("请输入：")
来源：https://cm.zhonguo5118.cn

PHP:  $name = trim(fgets(STDIN));
来源：https://jk.zhonguo5118.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：https://sg.zhonguo6118.cn

TS:   // Node.js：readline 模块
来源：https://zk.zhonguo5118.cn

Java: new Scanner(System.in).nextLine()
来源：https://cv.zhonguo6118.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：https://wk.zhonguo1118.cn

Ruby: gets.chomp
来源：https://cb.zhonguo4118.cn

C#:   Console.ReadLine();
来源：https://wb.zhonguo2118.cn

[A21] 保留指定小数位输出
来源：https://nk.zhonguo8118.cn

Py:   f"{3.14159:.2f}"
来源：https://uv.zhonguo8118.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：https://hp.zhonguo1118.cn

JS:   (3.14159).toFixed(2)
来源：https://hn.zhonguo8118.cn

TS:   (3.14159).toFixed(2)
来源：https://kg.zhonguo6118.cn

Java: String.format("%.2f", 3.14159)
来源：https://pe.zhonguo6118.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：https://ia.zhonguo2118.cn

Ruby: format("%.2f", 3.14159)
来源：https://mu.zhonguo2118.cn

C#:   3.14159.ToString("F2")
来源：https://qj.zhonguo7118.cn

[A22] 获取字符串长度
来源：https://fx.zhonguo8118.cn

Py:   len(s)
来源：https://yg.zhonguo6118.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：https://bt.zhonguo3118.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：https://kr.zhonguo8118.cn

TS:   s.length
来源：https://bx.zhonguo3118.cn

Java: s.length()
来源：https://qt.zhonguo4118.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：https://wy.zhonguo4118.cn

Ruby: s.length
来源：https://dz.zhonguo8118.cn

C#:   s.Length
来源：https://bp.zhonguo1118.cn

[A23] 大小写转换
来源：https://we.zhonguo8118.cn

Py:   s.upper(); s.lower(); s.title()
来源：https://yt.zhonguo7118.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：https://br.zhonguo4118.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：https://dn.zhonguo3118.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：https://mt.zhonguo1118.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：https://am.zhonguo4118.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：https://fu.zhonguo7118.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：https://wh.zhonguo7118.cn

C#:   s.ToUpper(); s.ToLower()
来源：https://rd.zhonguo6118.cn

[A24] 去除首尾空白
来源：https://wa.zhonguo3118.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：https://wy.zhonguo1118.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：https://we.zhonguo5118.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://dt.zhonguo7118.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://pl.zhonguo4118.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：https://oj.zhonguo1118.cn

Go:   strings.TrimSpace(s)
来源：https://mx.zhonguo8118.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：https://zy.zhonguo5118.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：https://uh.zhonguo5118.cn

[A25] 字符串比较
来源：https://yo.zhonguo7118.cn

Py:   s1 == s2; s1 != s2
来源：https://mb.zhonguo5118.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：https://rv.zhonguo7118.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：https://zw.zhonguo5118.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：https://rz.zhonguo4118.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：https://qq.zhonguo6118.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：https://xq.zhonguo8118.cn

Ruby: s1 == s2; s1 <=> s2
来源：https://or.zhonguo5118.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：https://tc.zhonguo7118.cn

[A26] 类型转换总览
来源：https://et.zhonguo5118.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：https://ic.zhonguo8118.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：https://vg.zhonguo5118.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：https://sw.zhonguo1118.cn

TS:   Number() String() Boolean() x as number
来源：https://ho.zhonguo7118.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：https://sp.zhonguo6118.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：https://qt.zhonguo7118.cn

Ruby: to_i to_f to_s to_sym to_a
来源：https://rs.zhonguo3118.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：https://lf.zhonguo8118.cn

================================================================================
来源：https://at.zhonguo4118.cn

B. 流程控制
来源：https://yk.zhonguo2118.cn

================================================================================
来源：https://kg.zhonguo6118.cn

[B01] 条件判断 if / else
来源：https://dm.zhonguo3118.cn

Py:   result = "正" if x > 0 else "非正"
来源：https://bi.zhonguo7118.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：https://jm.zhonguo8118.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：https://ve.zhonguo6118.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：https://mh.zhonguo5118.cn

Java: String r = x > 0 ? "正" : "非正";
来源：https://ov.zhonguo6118.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：https://no.zhonguo3118.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：https://zz.zhonguo5118.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：https://gw.zhonguo8118.cn

[B02] 多分支 else if / elif
来源：https://qu.zhonguo5118.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：https://ke.zhonguo6118.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：https://gg.zhonguo2118.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://iu.zhonguo7118.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://lj.zhonguo1118.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://mu.zhonguo6118.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：https://bb.zhonguo8118.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：https://li.zhonguo6118.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://ks.zhonguo1118.cn

[B03] switch / match / case
来源：https://pk.zhonguo8118.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：https://ic.zhonguo2118.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：https://lv.zhonguo7118.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://pv.zhonguo3118.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://pq.zhonguo7118.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：https://op.zhonguo6118.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：https://ac.zhonguo7118.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：https://bw.zhonguo5118.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：https://bc.zhonguo4118.cn

[B04] for 计数循环
来源：https://bm.zhonguo4118.cn

Py:   for i in range(10): print(i)
来源：https://dg.zhonguo2118.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：https://mx.zhonguo4118.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://xi.zhonguo3118.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://gh.zhonguo2118.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：https://ca.zhonguo1118.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：https://vf.zhonguo2118.cn

Ruby: 10.times { |i| puts i }
来源：https://kp.zhonguo3118.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：https://de.zhonguo5118.cn

[B05] 遍历数组 / 列表
来源：https://in.zhonguo5118.cn

Py:   for item in arr: print(item)
来源：https://sa.zhonguo7118.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：https://yh.zhonguo8118.cn

JS:   for (const item of arr) { console.log(item); }
来源：https://uz.zhonguo2118.cn

TS:   for (const item of arr) { console.log(item); }
来源：https://sd.zhonguo2118.cn

Java: for (var item : arr) { System.out.println(item); }
来源：https://yc.zhonguo1118.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：https://vb.zhonguo2118.cn

Ruby: arr.each { |item| puts item }
来源：https://fu.zhonguo5118.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：https://jp.zhonguo4118.cn

[B06] 遍历字典 / 对象
来源：https://xq.zhonguo5118.cn

Py:   for k, v in d.items(): print(k, v)
来源：https://er.zhonguo1118.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：https://ai.zhonguo3118.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://lu.zhonguo8118.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://gg.zhonguo1118.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：https://ew.zhonguo6118.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：https://mf.zhonguo8118.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：https://iy.zhonguo8118.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：https://lp.zhonguo8118.cn

[B07] while 循环
来源：https://vm.zhonguo3118.cn

Py:   while i < 10: i += 1
来源：https://hh.zhonguo4118.cn

PHP:  while ($i < 10) { $i++; }
来源：https://ry.zhonguo3118.cn

JS:   while (i < 10) { i++; }
来源：https://ee.zhonguo3118.cn

TS:   while (i < 10) { i++; }
来源：https://om.zhonguo2118.cn

Java: while (i < 10) { i++; }
来源：https://hv.zhonguo3118.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：https://lm.zhonguo4118.cn

Ruby: while i < 10; i += 1; end
来源：https://uj.zhonguo1118.cn

C#:   while (i < 10) { i++; }
来源：https://ki.zhonguo4118.cn

[B08] do-while（至少执行一次）
来源：https://xo.zhonguo5118.cn

Py:   # 无 do-while：用 while True + break
来源：https://od.zhonguo2118.cn

PHP:  do { $i++; } while ($i < 10);
来源：https://ol.zhonguo3118.cn

JS:   do { i++; } while (i < 10);
来源：https://wr.zhonguo4118.cn

TS:   do { i++; } while (i < 10);
来源：https://zi.zhonguo5118.cn

Java: do { i++; } while (i < 10);
来源：https://xz.zhonguo1118.cn

Go:   for { i++; if i >= 10 { break } }
来源：https://tz.zhonguo8118.cn

Ruby: begin; i += 1; end while i < 10
来源：https://by.zhonguo8118.cn

C#:   do { i++; } while (i < 10);
来源：https://av.zhonguo6118.cn

[B09] break 与 continue
来源：https://ki.zhonguo8118.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：https://tq.zhonguo4118.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：https://zs.zhonguo6118.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://nl.zhonguo5118.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://rh.zhonguo3118.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://wf.zhonguo6118.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：https://df.zhonguo7118.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：https://se.zhonguo2118.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://in.zhonguo1118.cn

[B10] 遍历同时拿索引
来源：https://ex.zhonguo1118.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：https://al.zhonguo3118.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：https://de.zhonguo1118.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：https://jw.zhonguo8118.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：https://ow.zhonguo3118.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：https://lj.zhonguo4118.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：https://vh.zhonguo1118.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：https://ha.zhonguo1118.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：https://fy.zhonguo8118.cn

[B11] 生成数字序列 / 区间
来源：https://iu.zhonguo8118.cn

Py:   list(range(0, 10, 2))
来源：https://th.zhonguo5118.cn

PHP:  range(0, 10, 2);
来源：https://df.zhonguo6118.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：https://lx.zhonguo4118.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：https://cv.zhonguo3118.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：https://uo.zhonguo2118.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：https://aw.zhonguo6118.cn

Ruby: (0...10).step(2).to_a
来源：https://gw.zhonguo5118.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：https://rs.zhonguo6118.cn

[B12] 跳出多层循环
来源：https://ig.zhonguo3118.cn

Py:   # 无标签跳转：抽成函数用 return
来源：https://cy.zhonguo4118.cn

PHP:  # 无标签：用 goto 或函数返回
来源：https://gm.zhonguo6118.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：https://vw.zhonguo2118.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：https://ob.zhonguo8118.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：https://xf.zhonguo3118.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：https://jm.zhonguo2118.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：https://ra.zhonguo1118.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：https://hp.zhonguo4118.cn

[B13] 判断是否为数字
来源：https://dx.zhonguo8118.cn

Py:   isinstance(x, (int, float))
来源：https://ut.zhonguo8118.cn

PHP:  is_numeric($x)
来源：https://fs.zhonguo8118.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：https://vn.zhonguo3118.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：https://ff.zhonguo8118.cn

Java: x instanceof Number
来源：https://rd.zhonguo3118.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：https://mo.zhonguo4118.cn

Ruby: x.is_a?(Numeric)
来源：https://ei.zhonguo8118.cn


<!-- 参考信息 -->