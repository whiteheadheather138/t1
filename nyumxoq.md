代发 wailian999

JS:   String(42); (42).toString()
来源：https://rs.zhonguo3118.cn

TS:   String(42)
来源：https://ss.zhonguo6118.cn

Java: String.valueOf(42); Integer.toString(42)
来源：https://ur.zhonguo6118.cn

Go:   strconv.Itoa(42)
来源：https://uk.zhonguo7118.cn

Ruby: 42.to_s
来源：https://ka.zhonguo5118.cn

C#:   42.ToString()
来源：https://wj.zhonguo2118.cn

[A08] 取整与四舍五入
来源：https://bl.zhonguo3118.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：https://ov.zhonguo5118.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：https://ih.zhonguo4118.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：https://aj.zhonguo3118.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：https://bg.zhonguo2118.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：https://ut.zhonguo1118.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：https://ro.zhonguo3118.cn

Ruby: 3.567.round(2); 3.9.floor
来源：https://mp.zhonguo4118.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：https://uf.zhonguo4118.cn

[A09] 绝对值与最大最小值
来源：https://dg.zhonguo2118.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：https://wb.zhonguo5118.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：https://ld.zhonguo7118.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：https://vv.zhonguo1118.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：https://vi.zhonguo8118.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：https://jo.zhonguo6118.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：https://yo.zhonguo5118.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：https://ku.zhonguo3118.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：https://vd.zhonguo1118.cn

[A10] 生成随机数
来源：https://yy.zhonguo7118.cn

Py:   import random; random.randint(1, 100)
来源：https://cw.zhonguo1118.cn

PHP:  random_int(1, 100);
来源：https://lv.zhonguo6118.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：https://wa.zhonguo4118.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：https://gl.zhonguo3118.cn

Java: new Random().nextInt(100) + 1
来源：https://vg.zhonguo3118.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：https://zr.zhonguo8118.cn

Ruby: rand(1..100)
来源：https://uc.zhonguo2118.cn

C#:   new Random().Next(1, 101)
来源：https://qk.zhonguo8118.cn

[A11] 条件表达式（三元）
来源：https://ye.zhonguo7118.cn

Py:   "yes" if x > 0 else "no"
来源：https://ep.zhonguo6118.cn

PHP:  $x > 0 ? "yes" : "no"
来源：https://bp.zhonguo6118.cn

JS:   x > 0 ? "yes" : "no"
来源：https://dc.zhonguo8118.cn

TS:   x > 0 ? "yes" : "no"
来源：https://cs.zhonguo2118.cn

Java: x > 0 ? "yes" : "no"
来源：https://th.zhonguo4118.cn

Go:   // 无三元运算符，需用 if 语句
来源：https://nf.zhonguo6118.cn

Ruby: x > 0 ? "yes" : "no"
来源：https://et.zhonguo8118.cn

C#:   x > 0 ? "yes" : "no"
来源：https://it.zhonguo7118.cn

[A12] 字符串插值 / 格式化
来源：https://qb.zhonguo6118.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：https://bb.zhonguo2118.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：https://ak.zhonguo5118.cn

JS:   `Hello, ${name}!`
来源：https://yj.zhonguo2118.cn

TS:   `Hello, ${name}!`
来源：https://ib.zhonguo8118.cn

Java: "Hello, %s!".formatted(name)
来源：https://kq.zhonguo1118.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：https://td.zhonguo2118.cn

Ruby: "Hello, #{name}!"
来源：https://ai.zhonguo1118.cn

C#:   $"Hello, {name}!"
来源：https://zs.zhonguo6118.cn

[A13] 多行字符串（练习 \n 转义）
来源：https://ax.zhonguo2118.cn

Py:   "第一行\n第二行"
来源：https://hd.zhonguo5118.cn

PHP:  "第一行\n第二行"
来源：https://lo.zhonguo3118.cn

JS:   "第一行\n第二行"
来源：https://fw.zhonguo7118.cn

TS:   "第一行\n第二行"
来源：https://eq.zhonguo3118.cn

Java: "第一行\n第二行"
来源：https://zk.zhonguo5118.cn

Go:   "第一行\n第二行"
来源：https://pb.zhonguo8118.cn

Ruby: "第一行\n第二行"
来源：https://ge.zhonguo1118.cn

C#:   "第一行\n第二行"
来源：https://zr.zhonguo7118.cn

[A14] 注释写法
来源：https://ja.zhonguo3118.cn

Py:   # 单行；三引号字符串可作多行说明
来源：https://zu.zhonguo6118.cn

PHP:  // 或 # 单行；/* 多行 */
来源：https://fa.zhonguo2118.cn

JS:   // 单行；/* 多行 */
来源：https://yk.zhonguo3118.cn

TS:   // 单行；/* 多行 */
来源：https://sj.zhonguo1118.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：https://yn.zhonguo6118.cn

Go:   // 单行；/* 多行 */
来源：https://ip.zhonguo6118.cn

Ruby: # 单行；=begin 多行 =end
来源：https://ji.zhonguo6118.cn

C#:   // 单行；/* 多行 */
来源：https://gx.zhonguo2118.cn

[A15] 空值判断与默认值
来源：https://xg.zhonguo5118.cn

Py:   value = data or "默认值"
来源：https://ck.zhonguo6118.cn

PHP:  $value = $data ?? "默认值";
来源：https://vs.zhonguo5118.cn

JS:   const value = data ?? "默认值";
来源：https://ao.zhonguo7118.cn

TS:   const value = data ?? "默认值";
来源：https://pf.zhonguo6118.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：https://ts.zhonguo7118.cn

Go:   if data == "" { data = "默认值" }
来源：https://xv.zhonguo6118.cn

Ruby: value = data || "默认值"
来源：https://hb.zhonguo8118.cn

C#:   var value = data ?? "默认值";
来源：https://al.zhonguo6118.cn

[A16] 真假值判断规则
来源：https://wx.zhonguo5118.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：https://ry.zhonguo5118.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：https://dw.zhonguo8118.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：https://lt.zhonguo6118.cn

TS:   if (!x) {}
来源：https://my.zhonguo4118.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：https://cc.zhonguo8118.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：https://gp.zhonguo5118.cn

Ruby: unless x            # nil 与 false 为假
来源：https://qy.zhonguo6118.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：https://ed.zhonguo6118.cn

[A17] 位运算
来源：https://kp.zhonguo5118.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://ng.zhonguo7118.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：https://lz.zhonguo7118.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://yo.zhonguo1118.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：https://hs.zhonguo7118.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://wi.zhonguo4118.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：https://rc.zhonguo6118.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://sy.zhonguo2118.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://ca.zhonguo2118.cn

[A18] 字符与 ASCII 码互转
来源：https://di.zhonguo3118.cn

Py:   ord("A"); chr(65)
来源：https://xy.zhonguo1118.cn

PHP:  ord("A"); chr(65)
来源：https://ki.zhonguo1118.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：https://ru.zhonguo4118.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：https://dy.zhonguo5118.cn

Java: (int) 'A'; (char) 65
来源：https://wu.zhonguo8118.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：https://du.zhonguo6118.cn

Ruby: "A".ord; 65.chr
来源：https://ag.zhonguo5118.cn

C#:   (int)'A'; (char)65
来源：https://mb.zhonguo3118.cn

[A19] 交换两个变量
来源：https://xf.zhonguo4118.cn

Py:   a, b = b, a
来源：https://zc.zhonguo3118.cn

PHP:  [$a, $b] = [$b, $a];
来源：https://ad.zhonguo8118.cn

JS:   [a, b] = [b, a];
来源：https://fb.zhonguo7118.cn

TS:   [a, b] = [b, a];
来源：https://gw.zhonguo4118.cn

Java: int t = a; a = b; b = t;
来源：https://kw.zhonguo1118.cn

Go:   a, b = b, a
来源：https://yb.zhonguo4118.cn

Ruby: a, b = b, a
来源：https://cf.zhonguo5118.cn

C#:   (a, b) = (b, a);
来源：https://is.zhonguo8118.cn

[A20] 读取标准输入
来源：https://kk.zhonguo7118.cn

Py:   name = input("请输入：")
来源：https://bx.zhonguo6118.cn

PHP:  $name = trim(fgets(STDIN));
来源：https://yo.zhonguo2118.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：https://ih.zhonguo6118.cn

TS:   // Node.js：readline 模块
来源：https://ou.zhonguo6118.cn

Java: new Scanner(System.in).nextLine()
来源：https://nq.zhonguo3118.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：https://ey.zhonguo2118.cn

Ruby: gets.chomp
来源：https://tv.zhonguo8118.cn

C#:   Console.ReadLine();
来源：https://ww.zhonguo3118.cn

[A21] 保留指定小数位输出
来源：https://jm.zhonguo7118.cn

Py:   f"{3.14159:.2f}"
来源：https://ww.zhonguo2118.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：https://zk.zhonguo6118.cn

JS:   (3.14159).toFixed(2)
来源：https://fc.zhonguo7118.cn

TS:   (3.14159).toFixed(2)
来源：https://zj.zhonguo8118.cn

Java: String.format("%.2f", 3.14159)
来源：https://mi.zhonguo3118.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：https://qy.zhonguo1118.cn

Ruby: format("%.2f", 3.14159)
来源：https://pz.zhonguo8118.cn

C#:   3.14159.ToString("F2")
来源：https://sk.zhonguo5118.cn

[A22] 获取字符串长度
来源：https://nb.zhonguo8118.cn

Py:   len(s)
来源：https://mr.zhonguo8118.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：https://ko.zhonguo8118.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：https://er.zhonguo1118.cn

TS:   s.length
来源：https://vc.zhonguo8118.cn

Java: s.length()
来源：https://ng.zhonguo2118.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：https://fn.zhonguo2118.cn

Ruby: s.length
来源：https://dp.zhonguo5118.cn

C#:   s.Length
来源：https://ka.zhonguo3118.cn

[A23] 大小写转换
来源：https://xd.zhonguo8118.cn

Py:   s.upper(); s.lower(); s.title()
来源：https://ue.zhonguo4118.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：https://wn.zhonguo6118.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：https://ry.zhonguo4118.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：https://ld.zhonguo4118.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：https://jn.zhonguo1118.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：https://cg.zhonguo4118.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：https://fo.zhonguo5118.cn

C#:   s.ToUpper(); s.ToLower()
来源：https://pj.zhonguo3118.cn

[A24] 去除首尾空白
来源：https://ja.zhonguo4118.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：https://dk.zhonguo8118.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：https://dw.zhonguo6118.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://mr.zhonguo1118.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://pt.zhonguo7118.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：https://ls.zhonguo1118.cn

Go:   strings.TrimSpace(s)
来源：https://sy.zhonguo7118.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：https://el.zhonguo2118.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：https://mf.zhonguo4118.cn

[A25] 字符串比较
来源：https://ph.zhonguo5118.cn

Py:   s1 == s2; s1 != s2
来源：https://cz.zhonguo3118.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：https://ik.zhonguo4118.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：https://fb.zhonguo1118.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：https://ov.zhonguo3118.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：https://wl.zhonguo7118.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：https://iz.zhonguo2118.cn

Ruby: s1 == s2; s1 <=> s2
来源：https://jy.zhonguo5118.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：https://wk.zhonguo3118.cn

[A26] 类型转换总览
来源：https://wg.zhonguo3118.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：https://gn.zhonguo2118.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：https://ij.zhonguo1118.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：https://oj.zhonguo8118.cn

TS:   Number() String() Boolean() x as number
来源：https://lu.zhonguo2118.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：https://fw.zhonguo8118.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：https://vg.zhonguo7118.cn

Ruby: to_i to_f to_s to_sym to_a
来源：https://ry.zhonguo1118.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：https://dk.zhonguo2118.cn

================================================================================
来源：https://di.zhonguo5118.cn

B. 流程控制
来源：https://ix.zhonguo7118.cn

================================================================================
来源：https://px.zhonguo5118.cn

[B01] 条件判断 if / else
来源：https://oh.zhonguo7118.cn

Py:   result = "正" if x > 0 else "非正"
来源：https://ga.zhonguo4118.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：https://tx.zhonguo2118.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：https://tn.zhonguo2118.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：https://fj.zhonguo3118.cn

Java: String r = x > 0 ? "正" : "非正";
来源：https://xc.zhonguo6118.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：https://bp.zhonguo1118.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：https://ib.zhonguo1118.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：https://tb.zhonguo1118.cn

[B02] 多分支 else if / elif
来源：https://kg.zhonguo6118.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：https://ma.zhonguo5118.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：https://tp.zhonguo2118.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://as.zhonguo2118.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://gh.zhonguo8118.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://ch.zhonguo5118.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：https://im.zhonguo7118.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：https://qp.zhonguo6118.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://nb.zhonguo3118.cn

[B03] switch / match / case
来源：https://tm.zhonguo6118.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：https://ar.zhonguo7118.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：https://pi.zhonguo1118.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://bq.zhonguo7118.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://nd.zhonguo2118.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：https://zc.zhonguo8118.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：https://so.zhonguo1118.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：https://mt.zhonguo5118.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：https://nh.zhonguo4118.cn

[B04] for 计数循环
来源：https://qq.zhonguo4118.cn

Py:   for i in range(10): print(i)
来源：https://dh.zhonguo3118.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：https://bo.zhonguo2118.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://ty.zhonguo6118.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://nn.zhonguo1118.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：https://pu.zhonguo3118.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：https://qv.zhonguo8118.cn

Ruby: 10.times { |i| puts i }
来源：https://nk.zhonguo7118.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：https://kh.zhonguo5118.cn

[B05] 遍历数组 / 列表
来源：https://eh.zhonguo6118.cn

Py:   for item in arr: print(item)
来源：https://rq.zhonguo6118.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：https://ut.zhonguo1118.cn

JS:   for (const item of arr) { console.log(item); }
来源：https://yx.zhonguo4118.cn

TS:   for (const item of arr) { console.log(item); }
来源：https://le.zhonguo6118.cn

Java: for (var item : arr) { System.out.println(item); }
来源：https://ft.zhonguo6118.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：https://oc.zhonguo7118.cn

Ruby: arr.each { |item| puts item }
来源：https://kd.zhonguo2118.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：https://oc.zhonguo4118.cn

[B06] 遍历字典 / 对象
来源：https://oe.zhonguo4118.cn

Py:   for k, v in d.items(): print(k, v)
来源：https://fu.zhonguo7118.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：https://uu.zhonguo8118.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://uv.zhonguo3118.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://na.zhonguo4118.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：https://xy.zhonguo1118.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：https://gy.zhonguo2118.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：https://um.zhonguo3118.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：https://le.zhonguo3118.cn

[B07] while 循环
来源：https://ko.zhonguo2118.cn

Py:   while i < 10: i += 1
来源：https://da.zhonguo5118.cn

PHP:  while ($i < 10) { $i++; }
来源：https://xt.zhonguo6118.cn

JS:   while (i < 10) { i++; }
来源：https://fr.zhonguo3118.cn

TS:   while (i < 10) { i++; }
来源：https://dm.zhonguo1118.cn

Java: while (i < 10) { i++; }
来源：https://km.zhonguo8118.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：https://fz.zhonguo3118.cn

Ruby: while i < 10; i += 1; end
来源：https://ku.zhonguo2118.cn

C#:   while (i < 10) { i++; }
来源：https://qx.zhonguo2118.cn

[B08] do-while（至少执行一次）
来源：https://td.zhonguo3118.cn

Py:   # 无 do-while：用 while True + break
来源：https://va.zhonguo2118.cn

PHP:  do { $i++; } while ($i < 10);
来源：https://ca.zhonguo5118.cn

JS:   do { i++; } while (i < 10);
来源：https://id.zhonguo5118.cn

TS:   do { i++; } while (i < 10);
来源：https://uc.zhonguo3118.cn

Java: do { i++; } while (i < 10);
来源：https://br.zhonguo2118.cn

Go:   for { i++; if i >= 10 { break } }
来源：https://xl.zhonguo6118.cn

Ruby: begin; i += 1; end while i < 10
来源：https://ue.zhonguo6118.cn

C#:   do { i++; } while (i < 10);
来源：https://sp.zhonguo1118.cn

[B09] break 与 continue
来源：https://df.zhonguo5118.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：https://cs.zhonguo8118.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：https://bd.zhonguo1118.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://yp.zhonguo2118.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://uv.zhonguo3118.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://nf.zhonguo2118.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：https://lx.zhonguo5118.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：https://nt.zhonguo6118.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://cq.zhonguo6118.cn

[B10] 遍历同时拿索引
来源：https://sb.zhonguo3118.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：https://gh.zhonguo5118.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：https://ii.zhonguo5118.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：https://yg.zhonguo8118.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：https://op.zhonguo4118.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：https://mu.zhonguo4118.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：https://iu.zhonguo6118.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：https://ku.zhonguo5118.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：https://un.zhonguo4118.cn

[B11] 生成数字序列 / 区间
来源：https://gy.zhonguo2118.cn

Py:   list(range(0, 10, 2))
来源：https://wc.zhonguo4118.cn

PHP:  range(0, 10, 2);
来源：https://wb.zhonguo4118.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：https://mp.zhonguo7118.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：https://my.zhonguo4118.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：https://ss.zhonguo4118.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：https://fc.zhonguo5118.cn

Ruby: (0...10).step(2).to_a
来源：https://au.zhonguo3118.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：https://yp.zhonguo7118.cn

[B12] 跳出多层循环
来源：https://dj.zhonguo6118.cn

Py:   # 无标签跳转：抽成函数用 return
来源：https://rv.zhonguo6118.cn

PHP:  # 无标签：用 goto 或函数返回
来源：https://kc.zhonguo5118.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：https://za.zhonguo7118.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：https://xv.zhonguo4118.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：https://lk.zhonguo1118.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：https://gv.zhonguo1118.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：https://zi.zhonguo2118.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：https://gd.zhonguo8118.cn

[B13] 判断是否为数字
来源：https://qk.zhonguo5118.cn

Py:   isinstance(x, (int, float))
来源：https://vm.zhonguo7118.cn

PHP:  is_numeric($x)
来源：https://xu.zhonguo2118.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：https://fx.zhonguo5118.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：https://zz.zhonguo7118.cn

Java: x instanceof Number
来源：https://dx.zhonguo2118.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：https://kq.zhonguo8118.cn

Ruby: x.is_a?(Numeric)
来源：https://yj.zhonguo7118.cn

C#:   x is int or double or decimal
来源：https://lx.zhonguo6118.cn

[B14] 判断值是否在集合内
来源：https://np.zhonguo2118.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：https://cv.zhonguo3118.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：https://df.zhonguo7118.cn


<!-- 参考信息 -->