代发 wailian999

[A10] 生成随机数
来源：https://fy.zhonguo1118.cn

Py:   import random; random.randint(1, 100)
来源：https://sg.zhonguo7118.cn

PHP:  random_int(1, 100);
来源：https://ax.zhonguo7118.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：https://fd.zhonguo7118.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：https://cp.zhonguo5118.cn

Java: new Random().nextInt(100) + 1
来源：https://qk.zhonguo5118.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：https://pr.zhonguo2118.cn

Ruby: rand(1..100)
来源：https://rn.zhonguo7118.cn

C#:   new Random().Next(1, 101)
来源：https://lj.zhonguo5118.cn

[A11] 条件表达式（三元）
来源：https://lo.zhonguo1118.cn

Py:   "yes" if x > 0 else "no"
来源：https://wt.zhonguo4118.cn

PHP:  $x > 0 ? "yes" : "no"
来源：https://lj.zhonguo2118.cn

JS:   x > 0 ? "yes" : "no"
来源：https://yo.zhonguo4118.cn

TS:   x > 0 ? "yes" : "no"
来源：https://aj.zhonguo1118.cn

Java: x > 0 ? "yes" : "no"
来源：https://qr.zhonguo6118.cn

Go:   // 无三元运算符，需用 if 语句
来源：https://iu.zhonguo4118.cn

Ruby: x > 0 ? "yes" : "no"
来源：https://ui.zhonguo5118.cn

C#:   x > 0 ? "yes" : "no"
来源：https://tq.zhonguo2118.cn

[A12] 字符串插值 / 格式化
来源：https://yw.zhonguo8118.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：https://ye.zhonguo8118.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：https://jg.zhonguo6118.cn

JS:   `Hello, ${name}!`
来源：https://yw.zhonguo3118.cn

TS:   `Hello, ${name}!`
来源：https://ez.zhonguo5118.cn

Java: "Hello, %s!".formatted(name)
来源：https://qc.zhonguo7118.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：https://ao.zhonguo4118.cn

Ruby: "Hello, #{name}!"
来源：https://eb.zhonguo3118.cn

C#:   $"Hello, {name}!"
来源：https://hh.zhonguo3118.cn

[A13] 多行字符串（练习 \n 转义）
来源：https://av.zhonguo6118.cn

Py:   "第一行\n第二行"
来源：https://nz.zhonguo6118.cn

PHP:  "第一行\n第二行"
来源：https://fy.zhonguo7118.cn

JS:   "第一行\n第二行"
来源：https://zj.zhonguo1118.cn

TS:   "第一行\n第二行"
来源：https://nz.zhonguo7118.cn

Java: "第一行\n第二行"
来源：https://yo.zhonguo1118.cn

Go:   "第一行\n第二行"
来源：https://mx.zhonguo2118.cn

Ruby: "第一行\n第二行"
来源：https://gx.zhonguo2118.cn

C#:   "第一行\n第二行"
来源：https://vx.zhonguo1118.cn

[A14] 注释写法
来源：https://yc.zhonguo7118.cn

Py:   # 单行；三引号字符串可作多行说明
来源：https://nt.zhonguo2118.cn

PHP:  // 或 # 单行；/* 多行 */
来源：https://ho.zhonguo8118.cn

JS:   // 单行；/* 多行 */
来源：https://ch.zhonguo2118.cn

TS:   // 单行；/* 多行 */
来源：https://xp.zhonguo6118.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：https://dw.zhonguo5118.cn

Go:   // 单行；/* 多行 */
来源：https://zp.zhonguo7118.cn

Ruby: # 单行；=begin 多行 =end
来源：https://bz.zhonguo2118.cn

C#:   // 单行；/* 多行 */
来源：https://ph.zhonguo6118.cn

[A15] 空值判断与默认值
来源：https://kg.zhonguo4118.cn

Py:   value = data or "默认值"
来源：https://xo.zhonguo6118.cn

PHP:  $value = $data ?? "默认值";
来源：https://zj.zhonguo3118.cn

JS:   const value = data ?? "默认值";
来源：https://ix.zhonguo5118.cn

TS:   const value = data ?? "默认值";
来源：https://bj.zhonguo5118.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：https://hr.zhonguo2118.cn

Go:   if data == "" { data = "默认值" }
来源：https://aw.zhonguo2118.cn

Ruby: value = data || "默认值"
来源：https://hj.zhonguo6118.cn

C#:   var value = data ?? "默认值";
来源：https://dz.zhonguo5118.cn

[A16] 真假值判断规则
来源：https://zq.zhonguo3118.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：https://rv.zhonguo1118.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：https://qy.zhonguo2118.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：https://pi.zhonguo2118.cn

TS:   if (!x) {}
来源：https://qm.zhonguo8118.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：https://by.zhonguo3118.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：https://ag.zhonguo8118.cn

Ruby: unless x            # nil 与 false 为假
来源：https://xy.zhonguo2118.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：https://oa.zhonguo6118.cn

[A17] 位运算
来源：https://yc.zhonguo4118.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://cs.zhonguo1118.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：https://yf.zhonguo1118.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://eu.zhonguo2118.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：https://cr.zhonguo6118.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://ev.zhonguo7118.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：https://dn.zhonguo6118.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://rf.zhonguo5118.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://lb.zhonguo2118.cn

[A18] 字符与 ASCII 码互转
来源：https://dn.zhonguo7118.cn

Py:   ord("A"); chr(65)
来源：https://zl.zhonguo2118.cn

PHP:  ord("A"); chr(65)
来源：https://xh.zhonguo5118.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：https://gm.zhonguo3118.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：https://ff.zhonguo3118.cn

Java: (int) 'A'; (char) 65
来源：https://qd.zhonguo6118.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：https://lp.zhonguo7118.cn

Ruby: "A".ord; 65.chr
来源：https://uq.zhonguo5118.cn

C#:   (int)'A'; (char)65
来源：https://xa.zhonguo6118.cn

[A19] 交换两个变量
来源：https://gr.zhonguo2118.cn

Py:   a, b = b, a
来源：https://lg.zhonguo1118.cn

PHP:  [$a, $b] = [$b, $a];
来源：https://me.zhonguo8118.cn

JS:   [a, b] = [b, a];
来源：https://wj.zhonguo2118.cn

TS:   [a, b] = [b, a];
来源：https://pk.zhonguo8118.cn

Java: int t = a; a = b; b = t;
来源：https://ax.zhonguo1118.cn

Go:   a, b = b, a
来源：https://zp.zhonguo7118.cn

Ruby: a, b = b, a
来源：https://ho.zhonguo7118.cn

C#:   (a, b) = (b, a);
来源：https://mp.zhonguo1118.cn

[A20] 读取标准输入
来源：https://jo.zhonguo2118.cn

Py:   name = input("请输入：")
来源：https://qi.zhonguo1118.cn

PHP:  $name = trim(fgets(STDIN));
来源：https://si.zhonguo8118.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：https://qs.zhonguo5118.cn

TS:   // Node.js：readline 模块
来源：https://zw.zhonguo1118.cn

Java: new Scanner(System.in).nextLine()
来源：https://hf.zhonguo1118.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：https://ym.zhonguo4118.cn

Ruby: gets.chomp
来源：https://yc.zhonguo1118.cn

C#:   Console.ReadLine();
来源：https://wb.zhonguo6118.cn

[A21] 保留指定小数位输出
来源：https://qj.zhonguo4118.cn

Py:   f"{3.14159:.2f}"
来源：https://hd.zhonguo6118.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：https://pg.zhonguo3118.cn

JS:   (3.14159).toFixed(2)
来源：https://dm.zhonguo5118.cn

TS:   (3.14159).toFixed(2)
来源：https://qs.zhonguo3118.cn

Java: String.format("%.2f", 3.14159)
来源：https://jx.zhonguo2118.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：https://ao.zhonguo5118.cn

Ruby: format("%.2f", 3.14159)
来源：https://ky.zhonguo5118.cn

C#:   3.14159.ToString("F2")
来源：https://ib.zhonguo8118.cn

[A22] 获取字符串长度
来源：https://eh.zhonguo4118.cn

Py:   len(s)
来源：https://fc.zhonguo5118.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：https://si.zhonguo5118.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：https://td.zhonguo5118.cn

TS:   s.length
来源：https://sr.zhonguo6118.cn

Java: s.length()
来源：https://ng.zhonguo6118.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：https://oz.zhonguo1118.cn

Ruby: s.length
来源：https://fh.zhonguo1118.cn

C#:   s.Length
来源：https://yz.zhonguo2118.cn

[A23] 大小写转换
来源：https://sl.zhonguo8118.cn

Py:   s.upper(); s.lower(); s.title()
来源：https://iu.zhonguo5118.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：https://uk.zhonguo2118.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：https://sj.zhonguo8118.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：https://aj.zhonguo1118.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：https://ia.zhonguo4118.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：https://bf.zhonguo7118.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：https://bp.zhonguo2118.cn

C#:   s.ToUpper(); s.ToLower()
来源：https://gy.zhonguo3118.cn

[A24] 去除首尾空白
来源：https://oe.zhonguo7118.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：https://kw.zhonguo7118.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：https://oj.zhonguo6118.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://kq.zhonguo6118.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://cs.zhonguo1118.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：https://ad.zhonguo1118.cn

Go:   strings.TrimSpace(s)
来源：https://fl.zhonguo6118.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：https://im.zhonguo8118.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：https://qq.zhonguo8118.cn

[A25] 字符串比较
来源：https://pk.zhonguo2118.cn

Py:   s1 == s2; s1 != s2
来源：https://it.zhonguo6118.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：https://vg.zhonguo5118.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：https://ju.zhonguo5118.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：https://lg.zhonguo4118.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：https://ge.zhonguo8118.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：https://nw.zhonguo3118.cn

Ruby: s1 == s2; s1 <=> s2
来源：https://cn.zhonguo4118.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：https://ao.zhonguo8118.cn

[A26] 类型转换总览
来源：https://gn.zhonguo2118.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：https://ni.zhonguo4118.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：https://ho.zhonguo1118.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：https://sy.zhonguo7118.cn

TS:   Number() String() Boolean() x as number
来源：https://vl.zhonguo2118.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：https://sd.zhonguo1118.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：https://lo.zhonguo6118.cn

Ruby: to_i to_f to_s to_sym to_a
来源：https://nj.zhonguo7118.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：https://vq.zhonguo7118.cn

================================================================================
来源：https://rf.zhonguo6118.cn

B. 流程控制
来源：https://lx.zhonguo2118.cn

================================================================================
来源：https://gn.zhonguo4118.cn

[B01] 条件判断 if / else
来源：https://si.zhonguo6118.cn

Py:   result = "正" if x > 0 else "非正"
来源：https://ef.zhonguo2118.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：https://xk.zhonguo8118.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：https://rp.zhonguo4118.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：https://gk.zhonguo3118.cn

Java: String r = x > 0 ? "正" : "非正";
来源：https://gn.zhonguo6118.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：https://ne.zhonguo4118.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：https://ym.zhonguo8118.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：https://vz.zhonguo3118.cn

[B02] 多分支 else if / elif
来源：https://qo.zhonguo8118.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：https://eg.zhonguo3118.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：https://pk.zhonguo3118.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://fn.zhonguo8118.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://mr.zhonguo8118.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://pf.zhonguo5118.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：https://nm.zhonguo2118.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：https://uu.zhonguo2118.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://fa.zhonguo1118.cn

[B03] switch / match / case
来源：https://nb.zhonguo2118.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：https://py.zhonguo3118.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：https://un.zhonguo5118.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://gj.zhonguo7118.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://rz.zhonguo6118.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：https://po.zhonguo2118.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：https://bu.zhonguo2118.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：https://ac.zhonguo1118.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：https://hb.zhonguo5118.cn

[B04] for 计数循环
来源：https://zc.zhonguo8118.cn

Py:   for i in range(10): print(i)
来源：https://fa.zhonguo7118.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：https://bu.zhonguo5118.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://ii.zhonguo8118.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://dt.zhonguo2118.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：https://ue.zhonguo1118.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：https://sc.zhonguo4118.cn

Ruby: 10.times { |i| puts i }
来源：https://kx.zhonguo1118.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：https://ao.zhonguo8118.cn

[B05] 遍历数组 / 列表
来源：https://id.zhonguo3118.cn

Py:   for item in arr: print(item)
来源：https://qj.zhonguo2118.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：https://jx.zhonguo5118.cn

JS:   for (const item of arr) { console.log(item); }
来源：https://ip.zhonguo8118.cn

TS:   for (const item of arr) { console.log(item); }
来源：https://sm.zhonguo8118.cn

Java: for (var item : arr) { System.out.println(item); }
来源：https://yj.zhonguo4118.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：https://kv.zhonguo4118.cn

Ruby: arr.each { |item| puts item }
来源：https://nk.zhonguo4118.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：https://pw.zhonguo2118.cn

[B06] 遍历字典 / 对象
来源：https://mk.zhonguo8118.cn

Py:   for k, v in d.items(): print(k, v)
来源：https://js.zhonguo2118.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：https://vd.zhonguo7118.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://rq.zhonguo6118.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://tf.zhonguo5118.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：https://wq.zhonguo6118.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：https://aa.zhonguo5118.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：https://sy.zhonguo7118.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：https://rh.zhonguo2118.cn

[B07] while 循环
来源：https://fj.zhonguo1118.cn

Py:   while i < 10: i += 1
来源：https://ww.zhonguo7118.cn

PHP:  while ($i < 10) { $i++; }
来源：https://ug.zhonguo4118.cn

JS:   while (i < 10) { i++; }
来源：https://ho.zhonguo5118.cn

TS:   while (i < 10) { i++; }
来源：https://ky.zhonguo6118.cn

Java: while (i < 10) { i++; }
来源：https://mm.zhonguo2118.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：https://hw.zhonguo8118.cn

Ruby: while i < 10; i += 1; end
来源：https://qm.zhonguo5118.cn

C#:   while (i < 10) { i++; }
来源：https://ht.zhonguo4118.cn

[B08] do-while（至少执行一次）
来源：https://zd.zhonguo6118.cn

Py:   # 无 do-while：用 while True + break
来源：https://ef.zhonguo1118.cn

PHP:  do { $i++; } while ($i < 10);
来源：https://mc.zhonguo8118.cn

JS:   do { i++; } while (i < 10);
来源：https://wi.zhonguo3118.cn

TS:   do { i++; } while (i < 10);
来源：https://th.zhonguo7118.cn

Java: do { i++; } while (i < 10);
来源：https://nt.zhonguo8118.cn

Go:   for { i++; if i >= 10 { break } }
来源：https://ca.zhonguo7118.cn

Ruby: begin; i += 1; end while i < 10
来源：https://vr.zhonguo8118.cn

C#:   do { i++; } while (i < 10);
来源：https://eh.zhonguo8118.cn

[B09] break 与 continue
来源：https://gd.zhonguo6118.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：https://mc.zhonguo8118.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：https://ef.zhonguo6118.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://sc.zhonguo4118.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://qh.zhonguo3118.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://ix.zhonguo2118.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：https://js.zhonguo2118.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：https://dr.zhonguo3118.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://er.zhonguo2118.cn

[B10] 遍历同时拿索引
来源：https://ue.zhonguo3118.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：https://ge.zhonguo2118.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：https://uk.zhonguo1118.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：https://hp.zhonguo2118.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：https://yg.zhonguo2118.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：https://hz.zhonguo1118.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：https://rb.zhonguo8118.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：https://qk.zhonguo3118.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：https://le.zhonguo8118.cn

[B11] 生成数字序列 / 区间
来源：https://mw.zhonguo4118.cn

Py:   list(range(0, 10, 2))
来源：https://rt.zhonguo5118.cn

PHP:  range(0, 10, 2);
来源：https://yr.zhonguo2118.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：https://zc.zhonguo4118.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：https://wv.zhonguo1118.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：https://nr.zhonguo6118.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：https://kh.zhonguo4118.cn

Ruby: (0...10).step(2).to_a
来源：https://jr.zhonguo5118.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：https://vr.zhonguo7118.cn

[B12] 跳出多层循环
来源：https://kf.zhonguo1118.cn

Py:   # 无标签跳转：抽成函数用 return
来源：https://kq.zhonguo5118.cn

PHP:  # 无标签：用 goto 或函数返回
来源：https://qt.zhonguo6118.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：https://fu.zhonguo5118.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：https://wl.zhonguo8118.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：https://jl.zhonguo4118.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：https://oz.zhonguo7118.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：https://xm.zhonguo3118.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：https://xu.zhonguo6118.cn

[B13] 判断是否为数字
来源：https://aw.zhonguo4118.cn

Py:   isinstance(x, (int, float))
来源：https://lv.zhonguo2118.cn

PHP:  is_numeric($x)
来源：https://nk.zhonguo5118.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：https://mu.zhonguo7118.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：https://xs.zhonguo3118.cn

Java: x instanceof Number
来源：https://em.zhonguo4118.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：https://kg.zhonguo6118.cn

Ruby: x.is_a?(Numeric)
来源：https://pn.zhonguo8118.cn

C#:   x is int or double or decimal
来源：https://hk.zhonguo3118.cn

[B14] 判断值是否在集合内
来源：https://gg.zhonguo6118.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：https://qw.zhonguo2118.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：https://ml.zhonguo3118.cn

JS:   [1, 2, 3].includes(x)
来源：https://ev.zhonguo5118.cn

TS:   [1, 2, 3].includes(x)
来源：https://kd.zhonguo5118.cn

Java: List.of(1, 2, 3).contains(x)
来源：https://ya.zhonguo2118.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：https://eh.zhonguo5118.cn

Ruby: [1, 2, 3].include?(x)
来源：https://dn.zhonguo2118.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：https://uu.zhonguo4118.cn

[B15] 布尔运算与取反
来源：https://bz.zhonguo3118.cn

Py:   a and b or not c
来源：https://hu.zhonguo2118.cn

PHP:  $a && $b || !$c
来源：https://pv.zhonguo3118.cn

JS:   a && b || !c
来源：https://np.zhonguo3118.cn

TS:   a && b || !c
来源：https://se.zhonguo2118.cn

Java: a && b || !c
来源：https://il.zhonguo2118.cn

Go:   a && b || !c
来源：https://qz.zhonguo3118.cn

Ruby: a && b || !c
来源：https://cw.zhonguo1118.cn

C#:   a && b || !c
来源：https://my.zhonguo8118.cn

[B16] 卫语句：不满足条件提前返回
来源：https://ud.zhonguo6118.cn

Py:   if not data: return
来源：https://nn.zhonguo3118.cn

PHP:  if (!$data) { return; }
来源：https://bn.zhonguo2118.cn

JS:   if (!data) return;
来源：https://mi.zhonguo1118.cn

TS:   if (!data) return;
来源：https://az.zhonguo7118.cn

Java: if (data == null) return;
来源：https://in.zhonguo5118.cn

Go:   if data == nil { return }
来源：https://wp.zhonguo5118.cn

Ruby: return if data.nil?
来源：https://bx.zhonguo4118.cn

C#:   if (data == null) return;
来源：https://pi.zhonguo8118.cn


<!-- 参考信息 -->